---
title: PRT-s probléma elhárítása
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573717"
---
# <a name="troubleshoot-prt-issue"></a><span data-ttu-id="6e7e7-102">PRT-s probléma elhárítása</span><span class="sxs-lookup"><span data-stu-id="6e7e7-102">Troubleshoot PRT issue</span></span>

<span data-ttu-id="6e7e7-103">Ahhoz, hogy bármilyen eszköz hitelesítve legyen, teljes mértékben be kell jegyeztetni, és jó állapotban kell lennie, és az elsődleges frissítési tokent (PRT) meg kell szereznie.</span><span class="sxs-lookup"><span data-stu-id="6e7e7-103">For any device to complete getting authenticated, it must be fully registered and in good state and able to acquire a Primary Refresh Token (PRT).</span></span>

<span data-ttu-id="6e7e7-104">A hibrid Azure AD csatlakozás regisztrációs folyamathoz az eszközöknek vállalati hálózaton kell lenniük.</span><span class="sxs-lookup"><span data-stu-id="6e7e7-104">The hybrid Azure AD join registration process requires devices to be on a corporate network.</span></span> <span data-ttu-id="6e7e7-105">Ez a funkció többek között a VPN-en is működik, de van némi kikötése.</span><span class="sxs-lookup"><span data-stu-id="6e7e7-105">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="6e7e7-106">Hallottuk, hogy az ügyfelek segítségre szorulnak a hibrid Azure AD-csatlakozás regisztrációjának hibaelhárításához a távoli munka körülményei között.</span><span class="sxs-lookup"><span data-stu-id="6e7e7-106">We’ve heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote-work circumstances.</span></span> <span data-ttu-id="6e7e7-107">Az alábbiakban felsoroljuk, hogy mi történik a regisztrációs folyamat során a motorháztető alatt.</span><span class="sxs-lookup"><span data-stu-id="6e7e7-107">Here’s a breakdown of what’s happening ‘under the hood’ during the registration process.</span></span>

<span data-ttu-id="6e7e7-108">**Felhőalapú hitelesítési környezet (az Azure AD Password hash szinkronizálása vagy a továbbítás hitelesítése)**</span><span class="sxs-lookup"><span data-stu-id="6e7e7-108">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="6e7e7-109">Ez a regisztrációs folyamat "szinkronizálási csatlakozás" néven is ismert.</span><span class="sxs-lookup"><span data-stu-id="6e7e7-109">This registration flow is also known as “Sync Join”.</span></span>

1. <span data-ttu-id="6e7e7-110">A Windows 10 a felhasználó által az eszközre való bejelentkezéskor megtalál egy SCP-rekordot.</span><span class="sxs-lookup"><span data-stu-id="6e7e7-110">Windows 10 discovers an SCP record upon user logging on to the device.</span></span>
    1. <span data-ttu-id="6e7e7-111">Az eszköz először az ügyféloldali SCP-ből kísérli meg beolvasni a bérlői adatokat a beállításjegyzékben [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="6e7e7-111">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="6e7e7-112">További információt ebben a [dokumentumban](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)talál.</span><span class="sxs-lookup"><span data-stu-id="6e7e7-112">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    2. <span data-ttu-id="6e7e7-113">Ha nem működik, az eszköz a helyszíni Active Directoryval (AD) kommunikál a bérlői adatok eléréséhez a Service Connection Pointból (SCP).</span><span class="sxs-lookup"><span data-stu-id="6e7e7-113">If it fails, the device communicates with on-premises Active Directory (AD) to get tenant information from Service Connection Point (SCP).</span></span> <span data-ttu-id="6e7e7-114">A SZOLGÁLTATÁSKAPCSOLÓDÁSI pont ellenőrzéséhez olvassa el ezt a [dokumentumot](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="6e7e7-114">To verify SCP, please refer to this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span> 

> [!NOTE]
> <span data-ttu-id="6e7e7-115">Javasoljuk, hogy engedélyezze az SCP használatát a HIRDETÉSben, és csak az ügyféloldali szolgáltatáskapcsolódási pontok használatát a kezdeti ellenőrzéshez.</span><span class="sxs-lookup"><span data-stu-id="6e7e7-115">We recommend enabling SCP in the AD and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="6e7e7-116">A Windows 10 a rendszerkörnyezetben próbál meg kommunikálni az Azure AD szolgáltatással, és az Azure AD-ot használva hitelesíti magát.</span><span class="sxs-lookup"><span data-stu-id="6e7e7-116">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span> <span data-ttu-id="6e7e7-117">Ellenőrizheti, hogy az eszköz hozzáférhet-e a Microsoft-erőforrásokhoz a rendszerfiók csoportban a számítógép-nyilvántartási csatlakozási parancsfájl használatával.</span><span class="sxs-lookup"><span data-stu-id="6e7e7-117">You can verify if the device can access Microsoft resources under the system account by using the Test Device Registration Connectivity script.</span></span>

3. <span data-ttu-id="6e7e7-118">A Windows 10 létrehoz egy önaláírt tanúsítványt, és a számítógép-objektum alatt tárolja a helyszíni hirdetések között.</span><span class="sxs-lookup"><span data-stu-id="6e7e7-118">Windows 10 generates a self-signed certificate and stores it under the computer object in on-premises AD.</span></span> <span data-ttu-id="6e7e7-119">Ehhez a tartományvezérlőt kell megadnia.</span><span class="sxs-lookup"><span data-stu-id="6e7e7-119">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="6e7e7-120">A tanúsítványt tartalmazó eszköz-objektum az Azure ad Connect segítségével szinkronizálódik az Azure AD-kapcsolaton keresztül.</span><span class="sxs-lookup"><span data-stu-id="6e7e7-120">A device object that has a certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="6e7e7-121">A szinkronizálási ciklus alapértelmezés szerint 30 percenként van, de az Azure AD Connect konfigurációjától függ.</span><span class="sxs-lookup"><span data-stu-id="6e7e7-121">Sync cycle is every 30 minutes by default, but it depends on configuration of Azure AD Connect.</span></span> <span data-ttu-id="6e7e7-122">További információért olvassa el ezt a [dokumentumot](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="6e7e7-122">For more information, please refer to this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="6e7e7-123">Ebben a szakaszban látnia kell a tárgy eszközt "függőben" állapotban az Azure-portál eszköz Blade területén.</span><span class="sxs-lookup"><span data-stu-id="6e7e7-123">At this stage, you should be able to see the subject device in “Pending” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="6e7e7-124">A Windows 10 rendszer következő felhasználó bejelentkezésekor a regisztráció be lesz töltve.</span><span class="sxs-lookup"><span data-stu-id="6e7e7-124">At the next user login to Windows 10, the registration will be completed.</span></span> 

> [!NOTE]
> <span data-ttu-id="6e7e7-125">Ha a VPN-en tartózkodik, és a kijelentkezési bejelentkezési folyamat lemondja a tartomány kapcsolatát, a regisztrációt kézzel is aktiválhatja:</span><span class="sxs-lookup"><span data-stu-id="6e7e7-125">If you're on VPN and a logoff-login process terminates the domain connectivity, you can trigger registration manually:</span></span>
 1. <span data-ttu-id="6e7e7-126">Dsregcmd/JOIN a rendszergazdától, vagy távolról a PSExec-on keresztül a számítógépre.</span><span class="sxs-lookup"><span data-stu-id="6e7e7-126">Issue a dsregcmd /join locally on admin prompt or remotely via PSExec to your PC.</span></span> <span data-ttu-id="6e7e7-127">Például PsExec-s \\ win10client01 cmd, dsregcmd/JOIN</span><span class="sxs-lookup"><span data-stu-id="6e7e7-127">For example, PsExec -s \\win10client01 cmd, dsregcmd /join</span></span>

 2. <span data-ttu-id="6e7e7-128">A hibrid kapcsolódási problémákkal kapcsolatos további részletekért olvassa el az [eszközökkel kapcsolatos problémák elhárítása](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)című témakört.</span><span class="sxs-lookup"><span data-stu-id="6e7e7-128">For more details on Hybrid Join issues, see [Troubleshoot devices Issue](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span></span>
