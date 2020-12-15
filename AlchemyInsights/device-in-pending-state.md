---
title: Eszköz függőben állapotban
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49678482"
---
# <a name="device-in-pending-state"></a><span data-ttu-id="fb252-102">Eszköz függőben állapotban</span><span class="sxs-lookup"><span data-stu-id="fb252-102">Device in pending state</span></span>

<span data-ttu-id="fb252-103">**Előfeltételek**</span><span class="sxs-lookup"><span data-stu-id="fb252-103">**Prerequisites:**</span></span>

1. <span data-ttu-id="fb252-104">Ha első alkalommal állítja be az eszközök regisztrációját, győződjön meg arról, hogy az Azure Active Directory-ban az Azure Active Directory-ban áttekintheti az [eszközillesztők bevezetését](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) , amely bemutatja, hogy miként szerezhet be eszközöket az Azure ad felügyelete alá.</span><span class="sxs-lookup"><span data-stu-id="fb252-104">If you are setting up device registrations for the first time, please ensure that you have reviewed [Introduction to device management in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) that will guide you on how to get devices under the control of Azure AD.</span></span>
2. <span data-ttu-id="fb252-105">Ha közvetlenül az Azure AD-ba jelentkezik be, és beiratkozik őket a Intune-ba, gondoskodnia kell arról, hogy az Intune-t [konfigurálta](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) , és először a [licencet](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) állítsa be.</span><span class="sxs-lookup"><span data-stu-id="fb252-105">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
3. <span data-ttu-id="fb252-106">Ellenőrizze, hogy jogosult-e műveletek végrehajtására az Azure AD-ban és a helyszíni AD-ban.</span><span class="sxs-lookup"><span data-stu-id="fb252-106">Ensure you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="fb252-107">Az Azure AD szolgáltatásban csak egy globális rendszergazda kezelhetik az eszközök regisztrációjának beállításait.</span><span class="sxs-lookup"><span data-stu-id="fb252-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="fb252-108">Ha a helyszíni Active Directoryban automatikus regisztrációkat állít be, az Active Directory és az Active Directory összevonási szolgáltatások (ha szükséges) rendszergazdájának kell lennie.</span><span class="sxs-lookup"><span data-stu-id="fb252-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="fb252-109">A hibrid Azure AD csatlakozás regisztrációs folyamathoz a vállalati hálózatban lévő eszközökre van szükség.</span><span class="sxs-lookup"><span data-stu-id="fb252-109">The hybrid Azure AD join registration process requires devices to be on corporate network.</span></span> <span data-ttu-id="fb252-110">Ez a funkció többek között a VPN-en is működik, de van némi kikötése.</span><span class="sxs-lookup"><span data-stu-id="fb252-110">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="fb252-111">Hallottuk, hogy az ügyfelek segítségre szorulnak a hibrid Azure AD-csatlakozás regisztrációs folyamatának hibaelhárítása távoli munkakörülmények között.</span><span class="sxs-lookup"><span data-stu-id="fb252-111">We have heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote work circumstances.</span></span>

<span data-ttu-id="fb252-112">**Felhőalapú hitelesítési környezet (az Azure AD Password hash szinkronizálása vagy a továbbítás hitelesítése)**</span><span class="sxs-lookup"><span data-stu-id="fb252-112">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="fb252-113">Ez a regisztrációs folyamat "szinkronizálási csatlakozás" néven is ismert.</span><span class="sxs-lookup"><span data-stu-id="fb252-113">This registration flow is also known as “Sync Join”.</span></span>

<span data-ttu-id="fb252-114">Itt megtudhatja, hogy mi történik a regisztrációs folyamat során:</span><span class="sxs-lookup"><span data-stu-id="fb252-114">Here is a breakdown of what happens during the registration process:</span></span>

1. <span data-ttu-id="fb252-115">A Windows 10 feltárta a Service Connection Point (SCP) rekordját, amikor a felhasználó bejelentkezik az eszközre.</span><span class="sxs-lookup"><span data-stu-id="fb252-115">Windows 10 discovers Service Connection Point (SCP) record when the user logs on to the device.</span></span>

    1. <span data-ttu-id="fb252-116">Az eszköz először az ügyféloldali SCP-ből kísérli meg beolvasni a bérlői adatokat a beállításjegyzékben [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="fb252-116">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="fb252-117">További információt a [dokumentum](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)című témakörben találhat.</span><span class="sxs-lookup"><span data-stu-id="fb252-117">For more information, see [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    1. <span data-ttu-id="fb252-118">Ha nem működik, az eszköz a helyszíni Active Directoryval kommunikál a bérlői adatoknak a SZOLGÁLTATÁSKAPCSOLÓDÁSI pontból való beszerzéséhez.</span><span class="sxs-lookup"><span data-stu-id="fb252-118">If it fails, the device communicates with on-premises Active Directory to get tenant information from SCP.</span></span> <span data-ttu-id="fb252-119">A SZOLGÁLTATÁSKAPCSOLÓDÁSI pont ellenőrzéséhez tekintse át ezt a [dokumentumot](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="fb252-119">To verify SCP, refer this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span>

    > [!NOTE]
    > <span data-ttu-id="fb252-120">Javasoljuk, hogy engedélyezze az SCP használatát az Active Directoryban, és csak ügyféloldali szolgáltatáskapcsolódási pontok használatát a kezdeti ellenőrzéshez.</span><span class="sxs-lookup"><span data-stu-id="fb252-120">We recommend enabling SCP in the Active Directory and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="fb252-121">A Windows 10 a rendszerkörnyezetben próbál meg kommunikálni az Azure AD szolgáltatással, és az Azure AD-ot használva hitelesíti magát.</span><span class="sxs-lookup"><span data-stu-id="fb252-121">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span>

    <span data-ttu-id="fb252-122">Ellenőrizheti, hogy az eszköz hozzáférhet-e a Microsoft-erőforrásokhoz a rendszerfiók csoportban a számítógép- [nyilvántartási csatlakozási parancsfájl](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0)használatával.</span><span class="sxs-lookup"><span data-stu-id="fb252-122">You can verify if the device can access Microsoft resources under the system account by using the [Test Device Registration Connectivity script](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span></span>

3. <span data-ttu-id="fb252-123">A Windows 10 önaláírt tanúsítványt hoz létre, és a számítógép-objektum alatt tárolja a helyszíni Active Directoryban.</span><span class="sxs-lookup"><span data-stu-id="fb252-123">Windows 10 generates self-signed certificate and stores it under the computer object in on-premises Active Directory.</span></span> <span data-ttu-id="fb252-124">Ehhez a tartományvezérlőt kell megadnia.</span><span class="sxs-lookup"><span data-stu-id="fb252-124">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="fb252-125">A tanúsítványt tartalmazó eszköz-objektum az Azure ad Connecten keresztül szinkronizálódik az Azure AD-hoz.</span><span class="sxs-lookup"><span data-stu-id="fb252-125">Device object that has certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="fb252-126">A szinkronizálási ciklus alapértelmezés szerint minden 30 perc, de az Azure AD Connect konfigurációjától függ.</span><span class="sxs-lookup"><span data-stu-id="fb252-126">Sync cycle is every 30 minutes by default, but it depends on the configuration of Azure AD Connect.</span></span> <span data-ttu-id="fb252-127">További információért olvassa el ezt a [dokumentumot](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="fb252-127">For more information, refer this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="fb252-128">Ebben a szakaszban látnia kell a tárgy eszközt "**függőben**" állapotban az Azure-portál eszköz Blade területén.</span><span class="sxs-lookup"><span data-stu-id="fb252-128">At this stage, you should be able to see the subject device in “**Pending**” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="fb252-129">A Windows 10 rendszer következő felhasználó bejelentkezésekor a regisztráció be lesz töltve.</span><span class="sxs-lookup"><span data-stu-id="fb252-129">At the next user login to Windows 10, the registration will be completed.</span></span>

    > [!NOTE]
    > <span data-ttu-id="fb252-130">Ha a VPN és a kijelentkezés/bejelentkezés funkció lemondja a tartomány kapcsolatát, akkor a regisztrációt kézzel is aktiválhatja.</span><span class="sxs-lookup"><span data-stu-id="fb252-130">If you are on VPN and logoff/login terminates the domain connectivity, you can trigger registration manually.</span></span> <span data-ttu-id="fb252-131">Teendő:</span><span class="sxs-lookup"><span data-stu-id="fb252-131">To do that:</span></span>
    >
    > <span data-ttu-id="fb252-132">Az `dsregcmd /join` PSExec-on keresztül távolról, a számítógépén keresztül is kiadhatja a helyileg a rendszergazdát.</span><span class="sxs-lookup"><span data-stu-id="fb252-132">Issue a `dsregcmd /join` locally on admin prompt or remotely via PSExec to your PC.</span></span>
    >
    > <span data-ttu-id="fb252-133">Példa: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span><span class="sxs-lookup"><span data-stu-id="fb252-133">For example: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span></span>

<span data-ttu-id="fb252-134">Az Azure Active Directory-regisztrációval kapcsolatos gyakori problémák az [eszközök – gyakori kérdések](https://docs.microsoft.com/azure/active-directory/devices/faq)című témakörben olvashatók.</span><span class="sxs-lookup"><span data-stu-id="fb252-134">For common issues with Azure Active Directory device registration, see [Devices FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).</span></span>
