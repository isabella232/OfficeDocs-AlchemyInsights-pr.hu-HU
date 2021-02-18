---
title: Külső beállítások kezelése
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8322"
- "9003227"
ms.openlocfilehash: 7caf46f9988ddbcbb16c0a2751dbda85bd7da34c
ms.sourcegitcommit: 616ae0cbd5769e12ae428e00088840cf05e52b6a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/17/2021
ms.locfileid: "50294318"
---
# <a name="managing-external-settings"></a><span data-ttu-id="00f5d-102">Külső beállítások kezelése</span><span class="sxs-lookup"><span data-stu-id="00f5d-102">Managing External Settings</span></span>

<span data-ttu-id="00f5d-103">**Bejelentés**</span><span class="sxs-lookup"><span data-stu-id="00f5d-103">**Announcement**</span></span>

- <span data-ttu-id="00f5d-104">[A WebView-bejelentkezés 2021. január 4-től](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support)való támogatása a Google-tól.</span><span class="sxs-lookup"><span data-stu-id="00f5d-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span></span> <span data-ttu-id="00f5d-105">Annak tesztelése, hogy az alkalmazásokat érinti-e a Google kompatibilitás tesztelésére vonatkozó útmutatása</span><span class="sxs-lookup"><span data-stu-id="00f5d-105">Test whether your apps are affected by following Google’s guidance on testing compatibility</span></span>
- <span data-ttu-id="00f5d-106">Mindenképpen a rendszer webnézetét vagy a rendszerböngészőt használja, amikor felhasználóit fogyasztói Google-fiókkal jelentkezik be</span><span class="sxs-lookup"><span data-stu-id="00f5d-106">Make sure to use the system webview or the system browser when signing in your users with consumer Google accounts</span></span>

<span data-ttu-id="00f5d-107">**Meghívási beállítások kezelése**</span><span class="sxs-lookup"><span data-stu-id="00f5d-107">**Manage Invitation Settings**</span></span>

<span data-ttu-id="00f5d-108">Ellenőrizze, hogy [konfigurálta-e](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) a külső együttműködési beállításokat úgy, hogy a megfelelő személyek meghívókat tudjanak küldeni.</span><span class="sxs-lookup"><span data-stu-id="00f5d-108">Confirm that you have [configured the external collaboration settings](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) to allow the appropriate people to send invitations.</span></span>

<span data-ttu-id="00f5d-109">**Vendégfelhasználói hozzáférési engedélyek kezelése**</span><span class="sxs-lookup"><span data-stu-id="00f5d-109">**Manage Guest User Access Permissions**</span></span>

1. <span data-ttu-id="00f5d-110">A globális rendszergazdák az Azure Portalon keresztül kezelhetik a vendégelérési engedélyeket a címtárban a külső együttműködési beállítások lapon a vendégelérési engedélyek konfigurálásával.</span><span class="sxs-lookup"><span data-stu-id="00f5d-110">Global admins can manage guest access permissions in the directory through the Azure portal by configuring the guest access permissions on the External Collaboration Settings page.</span></span> <span data-ttu-id="00f5d-111">[További információ erről a beállításról.](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="00f5d-111">[Learn more about this setting](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
2. <span data-ttu-id="00f5d-112">Ha azt szeretné, hogy a vendégek hozzáférjenek a Teamshez vagy a SharePointhoz hasonló alkalmazásokhoz, győződjön meg arról, hogy úgy állította be ezeket az alkalmazásokat, hogy vendégelérést engedélyezzenek.</span><span class="sxs-lookup"><span data-stu-id="00f5d-112">If you would like your guests to access apps such as Teams or SharePoint, confirm that you've configured those apps to allow guest access.</span></span> <span data-ttu-id="00f5d-113">További információ a [Teams beállításairól és a](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) [SharePointról.](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="00f5d-113">Learn more about the [Teams settings](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) and [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="00f5d-114">**Meghívók konfigurálása:**</span><span class="sxs-lookup"><span data-stu-id="00f5d-114">**Configuring invitations:**</span></span>

- [<span data-ttu-id="00f5d-115">Külső együttműködés engedélyezése a B2B-ben, valamint a vendégek meghívására képes személyek kezelése</span><span class="sxs-lookup"><span data-stu-id="00f5d-115">Enable B2B external collaboration and manage who can invite guests</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="00f5d-116">Adott szervezetek felhasználóinak szóló meghívók engedélyezése vagy blokkolása</span><span class="sxs-lookup"><span data-stu-id="00f5d-116">Allow or block invitations to users from specific organizations</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="00f5d-117">**Az engedélyezett identitásszolgáltatók konfigurálása:**</span><span class="sxs-lookup"><span data-stu-id="00f5d-117">**Configuring allowed identity providers:**</span></span>

- [<span data-ttu-id="00f5d-118">Google Federation</span><span class="sxs-lookup"><span data-stu-id="00f5d-118">Google Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="00f5d-119">Közvetlen összevonás</span><span class="sxs-lookup"><span data-stu-id="00f5d-119">Direct Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="00f5d-120">Egyszeres pin-kód hitelesítése e-mailben</span><span class="sxs-lookup"><span data-stu-id="00f5d-120">Email one-time Passcode Authentication</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)
