---
title: Letiltott a feltételes hozzáférés tartományhoz kötött eszközzel
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/20/2021
ms.locfileid: "51036699"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a><span data-ttu-id="8dd84-102">Letiltott a feltételes hozzáférés tartományhoz kötött eszközzel</span><span class="sxs-lookup"><span data-stu-id="8dd84-102">I’m getting blocked by Conditional Access with domain joined device</span></span>

<span data-ttu-id="8dd84-103">**Erősen ajánlott eszközök**</span><span class="sxs-lookup"><span data-stu-id="8dd84-103">**Highly Recommended Tools**</span></span>

<span data-ttu-id="8dd84-104">[Eszközregisztrációs hibaelhárító eszköz](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – Ez az eszköz segít elhárítani a leggyakoribb eszközregisztrációs problémákat.</span><span class="sxs-lookup"><span data-stu-id="8dd84-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - The tool that helps in troubleshooting the most common device registration issues.</span></span>

<span data-ttu-id="8dd84-105">[Eszközregisztrációs kapcsolat tesztelése parancsprogram](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – Ez a parancsfájl segít biztosítani, hogy egy eszköz hozzáférjen a rendszerfiók eszközregisztrációs végpontjaihoz.</span><span class="sxs-lookup"><span data-stu-id="8dd84-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - The script that helps ensuring that a device can access Device Registration endpoints under the system account.</span></span>

<span data-ttu-id="8dd84-106">[Azure AD device cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) – Ez a parancsfájl lehetővé teszi a elavult eszközök keresését és kezelését a környezetében.</span><span class="sxs-lookup"><span data-stu-id="8dd84-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - The script that enables you to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="8dd84-107">Íme néhány gyakori ok, amiért előfordulhat, hogy a feltételes hozzáférés nem sikerül egy tartományhoz csatlakozott eszköz (hibrid Azure AD).</span><span class="sxs-lookup"><span data-stu-id="8dd84-107">Here are some common reasons why conditional access may be failing a device that has joined a domain (Hybrid Azure AD).</span></span>

1. <span data-ttu-id="8dd84-108">**Nincs Azure AD PRT** az eszközön – Meg kell győződni arról, hogy az eszközön Azure AD primary Refresh Token (PRT) van.</span><span class="sxs-lookup"><span data-stu-id="8dd84-108">**There’s no Azure AD PRT on the device** - You need to ensure that the device has Azure AD Primary Refresh Token (PRT).</span></span> <span data-ttu-id="8dd84-109">A PRT-ről további információt ebben a dokumentumban [található.](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)</span><span class="sxs-lookup"><span data-stu-id="8dd84-109">For more information about PRT, see this [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="8dd84-110">Az Azure AD PRT ellenőrzéséhez futtassa az eszközön a parancsot, és ellenőrizze, hogy az `dsregcmd/status` "AzureAdPrt" egyenlő-e az "IGEN" értékkel.</span><span class="sxs-lookup"><span data-stu-id="8dd84-110">To verify if you have Azure AD PRT, you can run `dsregcmd/status` command on the device and verify if “AzureAdPrt” equals “YES”.</span></span>

<span data-ttu-id="8dd84-111">Ha az "AzureAdPrt" a "NEM" szó, ellenőrizze az alábbiakat:</span><span class="sxs-lookup"><span data-stu-id="8dd84-111">If "AzureAdPrt" is "NO", check the following:</span></span>

- <span data-ttu-id="8dd84-112">Függetlenül attól, hogy összevont környezete van-e az **AD FS használatával,** és ez a környezet nem érhető el a felhasználók otthoni hálózataiból: Ebben az esetben gondoskodjon arról, hogy a "felhasználónévvel átietett" végpontok elérhetők legyenek az extranetből.</span><span class="sxs-lookup"><span data-stu-id="8dd84-112">**Whether you have a federated environment with AD FS, and it’s unreachable from your users’ home networks**: In this case, ensure that your "usernamemixed" endpoints are accessible from the extranet.</span></span> <span data-ttu-id="8dd84-113">Ha az AD FS VPN mögött van, győződjön meg arról, hogy a felhasználók csatlakoznak a VPN-hez, és újra bejelentkeznek az eszközre.</span><span class="sxs-lookup"><span data-stu-id="8dd84-113">If your AD FS is behind a VPN, ensure that the users connect to the VPN and re-login to the device.</span></span> <span data-ttu-id="8dd84-114">További információ ebben a [dokumentumban található.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains)</span><span class="sxs-lookup"><span data-stu-id="8dd84-114">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span></span>

- <span data-ttu-id="8dd84-115">**Hogy az eszköz TPM-eszköze** hibás-e, és így nem tudja hitelesíteni az eszközt: Ellenőrizze a "tpm.msc" ellenőrzőt, és ellenőrizze, hogy a TPM állapota "Ready" (Készen áll-e).</span><span class="sxs-lookup"><span data-stu-id="8dd84-115">**Whether the device’s TPM is faulty and thus cannot authenticate the device**: Check "tpm.msc" to see if the state of TPM is "Ready".</span></span> <span data-ttu-id="8dd84-116">Ha nem, futtassa, és hagyja, hogy az eszköz újra `dsregcmd/leave` csatlakozzon az Azure AD-hez.</span><span class="sxs-lookup"><span data-stu-id="8dd84-116">If not, run `dsregcmd/leave` and let the device re-join to Azure AD.</span></span> <span data-ttu-id="8dd84-117">Ezután próbálkozzon újra.</span><span class="sxs-lookup"><span data-stu-id="8dd84-117">Then, try again.</span></span> <span data-ttu-id="8dd84-118">További információ ebben a [dokumentumban található.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="8dd84-118">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>

- <span data-ttu-id="8dd84-119">**Külső identitásszolgáltatót használ,** amely nem támogatja a WS-Trust protokollt.</span><span class="sxs-lookup"><span data-stu-id="8dd84-119">**You’re using a 3rd party identity provider, which does not support WS-Trust protocol**.</span></span> <span data-ttu-id="8dd84-120">A dokumentumokban leírtak szerint a hibrid Azure AD-hez csatlakozású eszközök ebben az esetben nem működnek.</span><span class="sxs-lookup"><span data-stu-id="8dd84-120">As described in our docs, hybrid Azure AD-joined devices cannot work in this case.</span></span> <span data-ttu-id="8dd84-121">Kérjük, forduljon az identitásszolgáltatójához segítségért.</span><span class="sxs-lookup"><span data-stu-id="8dd84-121">Please work with your Identity provider for support.</span></span>

2. <span data-ttu-id="8dd84-122">A felhasználók a Chrome böngészőt **Windows 10-fiókok** vagy Office-bővítmény nélkül használják: A Chrome nem használja automatikusan a **PRT-t az AAD-hez vagy hibrid-AAD-hez** csatlakozású eszközökön: Ez bármilyen eszközalapú feltételes hozzáférési házirend sikertelenségéhez vezet, és a "Nem regisztrált eszköz" hibaüzenet jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="8dd84-122">**Users are using Chrome browser without the Windows 10 Accounts** or **Office extension Chrome does not automatically use the PRT on AAD-joined or hybrid-AAD-joined devices**: This leads to failure of any device-based Conditional Access policies, with “Unregistered device” error message displayed.</span></span> <span data-ttu-id="8dd84-123">A Chrome-böngésző megfelelő használatához az SCCM-en vagy az Intune-on keresztül telepítenie kell a "Windows 10-fiókok" vagy "Office-bővítmények a felhasználók Chrome böngészőjéhez" szoftvert.</span><span class="sxs-lookup"><span data-stu-id="8dd84-123">To use Chrome browser correctly, you must install the “Windows 10 Accounts” or "Office extension to the users’ Chrome browser" via SCCM or Intune.</span></span> <span data-ttu-id="8dd84-124">További információ ebben a [dokumentumban található.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)</span><span class="sxs-lookup"><span data-stu-id="8dd84-124">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

<span data-ttu-id="8dd84-125">Ha a bővítményt nem lehet távoli leküldéses módban leküldéses módban elvégezni, értesítse a felhasználókat, hogy a fenti bővítmények közül manuálisan telepítsék az alkalmazásokat az eszközalapú feltételes hozzáférés mögötti hozzáférés érdekében.</span><span class="sxs-lookup"><span data-stu-id="8dd84-125">If it’s not possible to push the extension remotely, notify users to manually install one of the above extensions to access applications behind device-based Conditional Access.</span></span> <span data-ttu-id="8dd84-126">További információ ebben a [dokumentumban található.](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites)</span><span class="sxs-lookup"><span data-stu-id="8dd84-126">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span></span>

3. <span data-ttu-id="8dd84-127">Az eszköz megfelelően hibrid Azure AD-hez csatlakozott, de véletlenül törlődött vagy le lett tiltva, akár az **Azure AD Connectben,** akár az Azure Portalon történt szinkronizálási változások miatt: Ebben az esetben az eszközobjektum a továbbiakban nem ismerhető fel teljesen összekapcsolt eszközként annak ellenére, hogy az "AzureAdJoined" és a "PRT" állapot érvényesként jelenik meg az eszközön.</span><span class="sxs-lookup"><span data-stu-id="8dd84-127">**The device was correctly hybrid Azure AD joined, but it was inadvertently deleted or disabled, either due to sync changes in Azure AD Connect or from the Azure portal**: If this happens, the device object is no longer recognized as a fully joined device even though the "AzureAdJoined" and "PRT" status show up as valid on the device.</span></span>

<span data-ttu-id="8dd84-128">A probléma megoldásához futtassa az érintett eszközökön, és hagyja, hogy újracsatlakoztassanak az `dsregcmd/leave` Azure AD-hez.</span><span class="sxs-lookup"><span data-stu-id="8dd84-128">To fix this issue, run `dsregcmd/leave` on the affected devices and let them rejoin Azure AD.</span></span> <span data-ttu-id="8dd84-129">További információ ebben a [dokumentumban található.](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices)</span><span class="sxs-lookup"><span data-stu-id="8dd84-129">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span></span>

> [!NOTE]
> <span data-ttu-id="8dd84-130">Ha eszközei Windows 10 1809-es frissítéssel, VPN/felhőproxyval vannak frissítve, és problémákat látnak az "AzureAdPrt" állapottal vagy bármilyen SSO-problémával rendelkező appban (az Outlook nem csatlakozik a postaládához a PRT használata nélkül), győződjön meg arról, hogy a [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) vagy az áprilisi kumulatív [frissítés KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) frissítést használva akadályozza meg a PRT-hibákat az ilyen gépeken.</span><span class="sxs-lookup"><span data-stu-id="8dd84-130">If your devices are on Windows 10, 1809 update, with VPN/Cloud Proxy and see issues with "AzureAdPrt" state or any app with SSO problem (outlook not connecting to mailbox even though you had PRT), ensure you have this patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) or April cumulative update [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) to prevent PRT failures on those machines.</span></span>

















