---
title: A jelszóvisszaírás nem működik
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
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243367"
---
# <a name="password-writeback-is-not-working"></a><span data-ttu-id="bd28b-102">A jelszóvisszaírás nem működik</span><span class="sxs-lookup"><span data-stu-id="bd28b-102">Password Writeback is not working</span></span>

<span data-ttu-id="bd28b-103">**Problémákat tapasztalok a jelszó-visszaírás konfigurálásával kapcsolatban**</span><span class="sxs-lookup"><span data-stu-id="bd28b-103">**I'm having problems configuring password writeback**</span></span>

- <span data-ttu-id="bd28b-104">A jelszóvisszaírás egy prémium funkció.</span><span class="sxs-lookup"><span data-stu-id="bd28b-104">Password writeback is a premium feature.</span></span>
- <span data-ttu-id="bd28b-105">Győződjön meg arról, hogy megértette a licencelési követelményeket:</span><span class="sxs-lookup"><span data-stu-id="bd28b-105">Make sure that you understand the licensing requirements:</span></span>
  - <span data-ttu-id="bd28b-106">A szervezetéhez legalább egy licencnek hozzá kell rendelnie</span><span class="sxs-lookup"><span data-stu-id="bd28b-106">You must have at least one license assigned in your organization</span></span>
  - <span data-ttu-id="bd28b-107">**Csak felhőbeli felhasználók** – Bármely Office 365 -ös (O365) fizetős termékváltozat vagy Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="bd28b-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
  - <span data-ttu-id="bd28b-108">**Felhőbeli és/vagy helyszíni** felhasználók – Azure AD Premium P1 vagy P2, Enterprise Mobility + Security (EMS) vagy Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="bd28b-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="bd28b-109">A licencelési követelményekről az [Azure AD önkiszolgáló jelszó-visszaállítási](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing) licencelési követelményeiben olvashat bővebben.</span><span class="sxs-lookup"><span data-stu-id="bd28b-109">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span></span>
- <span data-ttu-id="bd28b-110">Legalább egy rendszergazdai fiókkal és egy tesztfelhasználói fiókkal rendelkezik a megfelelő licenccel.</span><span class="sxs-lookup"><span data-stu-id="bd28b-110">You have at least one administrator account and one test user account with one of the appropriate license.</span></span>
- <span data-ttu-id="bd28b-111">A jelszó-visszaíráshoz csatlakoztatnia kell az Azure AD Connectet az elsődleges tartományvezérlő emulátorához.</span><span class="sxs-lookup"><span data-stu-id="bd28b-111">You must connect Azure AD Connect to the Primary Domain Controller Emulator for password writeback to work.</span></span> <span data-ttu-id="bd28b-112">Beállíthatja úgy az Azure AD Connectet, hogy  elsődleges tartományvezérlőt használjon. Kattintson a jobb gombbal az Active Directory szinkronizálási összekötő tulajdonságaira, és válassza a címtárpartíciók **konfigurálása parancsot.**</span><span class="sxs-lookup"><span data-stu-id="bd28b-112">You can configure Azure AD Connect to use a Primary Domain Controller by right clicking on the **properties** of the Active Directory synchronization connector, then selecting **configure directory partitions**.</span></span> <span data-ttu-id="bd28b-113">Itt keresse meg a **tartományvezérlő** kapcsolati beállításainak szakaszát, és jelölje be a jelölőnégyzetet, amely csak előnyben részesített **tartományvezérlőket használ.**</span><span class="sxs-lookup"><span data-stu-id="bd28b-113">From there, look for the **domain controller connection settings** section and check the box titled **only use preferred domain controllers**.</span></span>
  > [!NOTE]
  > <span data-ttu-id="bd28b-114">Ha az előnyben részesített tartományvezérlő nem PDC-emulátor, az Azure AD Connect továbbra is kapcsolatba fog lépjen a pdc-nek jelszó-visszaírásért.</span><span class="sxs-lookup"><span data-stu-id="bd28b-114">If the preferred DC is not a PDC emulator, Azure AD Connect will still reach out to the PDC for password writeback.</span></span>
- <span data-ttu-id="bd28b-115">A bérlői fiókban beállította és engedélyezte a jelszó-visszaállítást.</span><span class="sxs-lookup"><span data-stu-id="bd28b-115">Password reset has been configured and enabled in your tenant.</span></span> <span data-ttu-id="bd28b-116">További információt az Azure AD-jelszavak alaphelyzetbe állításának [engedélyezése a felhasználók számára.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)</span><span class="sxs-lookup"><span data-stu-id="bd28b-116">For more information, see [Enable users to reset their Azure AD passwords](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span></span>
- <span data-ttu-id="bd28b-117">Győződjön meg arról, hogy a jelszó-visszaírás engedélyezéséhez használt rendszergazdai fiók egy felhőbeli rendszergazdai fiók (amely nem helyszíni AD-ban jött létre az Azure AD-ban)</span><span class="sxs-lookup"><span data-stu-id="bd28b-117">Make sure that the administrator account being used to enable Password Writeback is a cloud administrator account (created in Azure AD not on-premises AD)</span></span>
- <span data-ttu-id="bd28b-118">A Windows Server 2008 R2, a Windows Server 2012 vagy a Windows Server 2012 R2 rendszert futtató helyszíni AD-telepítésben telepítve van a legújabb szervizcsomagok</span><span class="sxs-lookup"><span data-stu-id="bd28b-118">You have a single or multi-forest AD on-premises deployment running Windows Server 2008 R2, Windows Server 2012, or Windows Server 2012 R2 with the latest service packs installed</span></span>
- <span data-ttu-id="bd28b-119">Telepítve van az Azure AD Connect eszköz, és előkészítette az AD-környezetet a felhőbe való szinkronizáláshoz.</span><span class="sxs-lookup"><span data-stu-id="bd28b-119">You have the Azure AD Connect tool installed and you have prepared your AD environment for synchronization to the cloud.</span></span> <span data-ttu-id="bd28b-120">A jelszóvisszaírás tesztelése előtt győződjön meg arról, hogy először teljes körű importálást és teljes szinkronizálást végzett az Azure AD Connectben az AD és az Azure AD szolgáltatásból.</span><span class="sxs-lookup"><span data-stu-id="bd28b-120">Before testing password writeback, make sure that you first complete a full import and full sync from both AD and Azure AD in Azure AD Connect.</span></span>
- <span data-ttu-id="bd28b-121">További információ: teljes szinkronizálás és teljes importálás az [Azure AD Connectben](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span><span class="sxs-lookup"><span data-stu-id="bd28b-121">To learn more, see how to do a [full sync and full import in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span></span>

<span data-ttu-id="bd28b-122">**Probléma van a jelszó-visszaírási kapcsolattal**</span><span class="sxs-lookup"><span data-stu-id="bd28b-122">**I'm having a problem with password writeback connectivity**</span></span>

1. <span data-ttu-id="bd28b-123">Az Azure AD Connect legújabb [verziójának letöltése és engedélyezése](https://www.microsoft.com/download/details.aspx?id=47594)</span><span class="sxs-lookup"><span data-stu-id="bd28b-123">Download and enable the latest version of [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span></span>
2. <span data-ttu-id="bd28b-124">Tűzfalkonfiguráció: Az Azure AD Connect eszköznek (1.1.443-as vagy fenti) kimenő **HTTPS-hozzáférésre** van szüksége a következő szolgáltatásokhoz:</span><span class="sxs-lookup"><span data-stu-id="bd28b-124">Firewall configuration: The Azure AD Connect tool (1.1.443 and above) will need **outbound HTTPS** access to:</span></span>
    - <span data-ttu-id="bd28b-125">passwordreset.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="bd28b-125">passwordreset.microsoftonline.com</span></span>
    - <span data-ttu-id="bd28b-126">servicebus.windows.networks</span><span class="sxs-lookup"><span data-stu-id="bd28b-126">servicebus.windows.networks</span></span>
3. <span data-ttu-id="bd28b-127">Az üresjárati kapcsolatok megőrzésének engedélyezése legalább 2–3 percig</span><span class="sxs-lookup"><span data-stu-id="bd28b-127">Allow idle connections to persist for at least 2-3 minutes</span></span>

<span data-ttu-id="bd28b-128">**Továbbra is problémákat tapasztalok a jelszó-visszaírással kapcsolatban**</span><span class="sxs-lookup"><span data-stu-id="bd28b-128">**I'm still having problems with password writeback**</span></span>

- <span data-ttu-id="bd28b-129">Ha továbbra is nehézségekbe ütközik, próbálja meg letiltani és újra engedélyezni a jelszóvisszaírási szolgáltatást az Azure AD Connect eszközben</span><span class="sxs-lookup"><span data-stu-id="bd28b-129">If you are still having difficulty, try disabling and re-enabling the password writeback service in the Azure AD Connect tool</span></span>
- <span data-ttu-id="bd28b-130">További információ a [jelszóvisszaírás](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot) letiltásához és újra engedélyezéséhez</span><span class="sxs-lookup"><span data-stu-id="bd28b-130">To learn more, see how to [disable and re-enable password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span></span>
