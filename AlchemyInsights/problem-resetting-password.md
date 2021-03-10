---
title: Probléma a jelszó alaphelyzetbe állításával
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694377"
---
# <a name="problems-resetting-password"></a><span data-ttu-id="6a99f-102">Problémák a jelszó alaphelyzetbe állításával</span><span class="sxs-lookup"><span data-stu-id="6a99f-102">Problems resetting password</span></span>

<span data-ttu-id="6a99f-103">Az alábbiakban néhány olyan problémát talál, amely a jelszó alaphelyzetbe állításakor és a lehetséges megoldások során előfordulhat:</span><span class="sxs-lookup"><span data-stu-id="6a99f-103">Following are some of the issues that you might face when resetting password and the possible solutions:</span></span>

<span data-ttu-id="6a99f-104">**A jelszó-visszaállítás más kategóriákban nem szereplő problémáim vannak**</span><span class="sxs-lookup"><span data-stu-id="6a99f-104">**I'm having an issue with password reset not covered in the other categories**</span></span>

- <span data-ttu-id="6a99f-105">Győződjön meg arról, hogy jogosult a jelszavak alaphelyzetbe állításra.</span><span class="sxs-lookup"><span data-stu-id="6a99f-105">Ensure you are authorized to reset passwords.</span></span> <span data-ttu-id="6a99f-106">Csak a globális, a jelszó és a felhasználói rendszergazdák állíthatják alaphelyzetbe a felhasználói jelszavakat.</span><span class="sxs-lookup"><span data-stu-id="6a99f-106">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="6a99f-107">A globális rendszergazdák más jogosultsággal rendelkező rendszergazdák jelszavát is alaphelyzetbe állíthatják.</span><span class="sxs-lookup"><span data-stu-id="6a99f-107">Global administrators can also reset other privileged administrator's passwords.</span></span>
- <span data-ttu-id="6a99f-108">Győződjön meg arról, hogy megértette a licencelési követelményeket:</span><span class="sxs-lookup"><span data-stu-id="6a99f-108">Ensure that you understand the licensing requirements:</span></span>
    - <span data-ttu-id="6a99f-109">A szervezetéhez legalább egy licencnek hozzá kell rendelnie</span><span class="sxs-lookup"><span data-stu-id="6a99f-109">You must have at least one license assigned in your organization</span></span>
        - <span data-ttu-id="6a99f-110">Csak felhőbeli felhasználók – Bármely Office 365 -ös (O365) fizetős termékváltozat vagy Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="6a99f-110">Cloud only users - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
        - <span data-ttu-id="6a99f-111">Felhőbeli és/vagy helyszíni felhasználók – Azure AD Premium P1 vagy P2, Enterprise Mobility + Security (EMS) vagy Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="6a99f-111">Cloud and/or on-premises users - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
        - <span data-ttu-id="6a99f-112">A licencelési követelményekről az Azure AD önkiszolgáló jelszó-visszaállítási licenckövetelményei [között olvashat bővebben.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="6a99f-112">To read more about licensing requirements see the article [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="6a99f-113">**Problémákat tapasztalok a beállított jelszó-visszaállítási házirend tesztelése során**</span><span class="sxs-lookup"><span data-stu-id="6a99f-113">**I'm having problems testing the password reset policy I set**</span></span>

- <span data-ttu-id="6a99f-114">A legutóbb alkalmazott házirendek replikálása az összes adatközpontban és végponton néhány percig is eltarthat.</span><span class="sxs-lookup"><span data-stu-id="6a99f-114">Recently applied policies can take several minutes to replicate across all data centers and end-points.</span></span> <span data-ttu-id="6a99f-115">Az adatközponttól való fizikai távolság is befolyásolja, hogy milyen gyorsan alkalmazza a program a módosításokat.</span><span class="sxs-lookup"><span data-stu-id="6a99f-115">Physical distance from the data center will also affect how quickly changes are applied.</span></span>
- <span data-ttu-id="6a99f-116">Tesztelje a tesztet egy végfelhasználóval, ne rendszergazdával, és tesztelje a tesztelést néhány felhasználóval.</span><span class="sxs-lookup"><span data-stu-id="6a99f-116">Test with an end user, not an administrator, and pilot with a small set of users.</span></span> <span data-ttu-id="6a99f-117">Az Azure Portalon konfigurált házirendek csak a végfelhasználókra vonatkoznak, a rendszergazdákra nem.</span><span class="sxs-lookup"><span data-stu-id="6a99f-117">The policies configured in the Azure portal ONLY apply to end-users, not administrators.</span></span> <span data-ttu-id="6a99f-118">A Microsoft erős alapértelmezett kétoldali jelszó-visszaállítási házirendet érvényesít minden Azure-rendszergazdai szerepkörhöz (például: globális rendszergazda, ügyfélszolgálati rendszergazda, jelszókezelő stb.).</span><span class="sxs-lookup"><span data-stu-id="6a99f-118">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role (Example: Global Administrator, Helpdesk Administrator, Password Administrator, etc.)</span></span>
    - <span data-ttu-id="6a99f-119">További információ a [rendszergazdákra vonatkozó házirendekről.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)</span><span class="sxs-lookup"><span data-stu-id="6a99f-119">Learn more about [policies for administrators](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span></span>

<span data-ttu-id="6a99f-120">**Jelszó-visszaállítást szeretnék telepíteni, de nem szeretném, ha a felhasználóim további biztonsági adatokat regisztrálnak**</span><span class="sxs-lookup"><span data-stu-id="6a99f-120">**I want to deploy password reset but I don't want to make my users register additional security info**</span></span>

<span data-ttu-id="6a99f-121">Töltse ki előre a felhasználók adatait, hogy ne szükséges nekik!</span><span class="sxs-lookup"><span data-stu-id="6a99f-121">Pre-populate data for your users so they don't have to!</span></span> <span data-ttu-id="6a99f-122">Rendszergazdaként beállíthatja a telefon- és e-mail-tulajdonságokat a felhasználóknak, mielőtt jelszó-visszaállítást vezet be a szervezetében.</span><span class="sxs-lookup"><span data-stu-id="6a99f-122">- As an administrator you can set phone and email properties for your users before rolling out password reset to your organization.</span></span> <span data-ttu-id="6a99f-123">Ezt egy API, PowerShell vagy Azure AD Connect használatával tudja megtenni.</span><span class="sxs-lookup"><span data-stu-id="6a99f-123">You can do this using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="6a99f-124">További információ:</span><span class="sxs-lookup"><span data-stu-id="6a99f-124">More information here:</span></span>
- [<span data-ttu-id="6a99f-125">Jelszó-visszaállítás telepítése a felhasználók regisztrálásának előírása nélkül</span><span class="sxs-lookup"><span data-stu-id="6a99f-125">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [<span data-ttu-id="6a99f-126">A jelszó-visszaállítás által használt adatok</span><span class="sxs-lookup"><span data-stu-id="6a99f-126">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="6a99f-127">**A jelszó-visszaállítás gomb szürkével kiszürkül**</span><span class="sxs-lookup"><span data-stu-id="6a99f-127">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="6a99f-128">Ön nem jogosult a felhasználó jelszavának alaphelyzetbe állítania.</span><span class="sxs-lookup"><span data-stu-id="6a99f-128">You are not authorized to reset this user's passwords.</span></span> <span data-ttu-id="6a99f-129">Csak a globális, a jelszó és a felhasználói rendszergazdák állíthatják alaphelyzetbe a felhasználói jelszavakat.</span><span class="sxs-lookup"><span data-stu-id="6a99f-129">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="6a99f-130">A globális rendszergazdák más jogosultsággal rendelkező rendszergazdák jelszavát is alaphelyzetbe állíthatják.</span><span class="sxs-lookup"><span data-stu-id="6a99f-130">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="6a99f-131">**Nem látom a jelszó-visszaállítási panelt**</span><span class="sxs-lookup"><span data-stu-id="6a99f-131">**I don't see the password reset blade**</span></span>

<span data-ttu-id="6a99f-132">Ön nem jogosult a jelszavak alaphelyzetbe állításra.</span><span class="sxs-lookup"><span data-stu-id="6a99f-132">You are not authorized to reset passwords.</span></span> <span data-ttu-id="6a99f-133">Csak a globális, a jelszó és a felhasználói rendszergazdák állíthatják alaphelyzetbe a felhasználói jelszavakat.</span><span class="sxs-lookup"><span data-stu-id="6a99f-133">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="6a99f-134">A globális rendszergazdák más jogosultsággal rendelkező rendszergazdák jelszavát is alaphelyzetbe állíthatják.</span><span class="sxs-lookup"><span data-stu-id="6a99f-134">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="6a99f-135">**Nem látom a helyszíni integrációs panelt a jelszó-visszaállításban**</span><span class="sxs-lookup"><span data-stu-id="6a99f-135">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="6a99f-136">A helyszíni integrációs blade csak hibrid környezetekben jelenik meg – ami azt jelenti, hogy jelszóvisszaírást használ a helyszíni felhasználók jelszavának a módosítása érdekében.</span><span class="sxs-lookup"><span data-stu-id="6a99f-136">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>
- <span data-ttu-id="6a99f-137">A következő esetben nem látja ezt a blade-et:</span><span class="sxs-lookup"><span data-stu-id="6a99f-137">You do not see this blade if:</span></span>
    - <span data-ttu-id="6a99f-138">Nem használ jelszó-visszaírást</span><span class="sxs-lookup"><span data-stu-id="6a99f-138">You are not using password writeback</span></span>
    - <span data-ttu-id="6a99f-139">Probléma van a jelszó-visszaírás telepítésével/csatlakoztatásával</span><span class="sxs-lookup"><span data-stu-id="6a99f-139">There is a problem with your installation/connectivity of password writeback</span></span>
    - <span data-ttu-id="6a99f-140">Probléma van az Azure AD Connect telepítésével/csatlakoztatásával</span><span class="sxs-lookup"><span data-stu-id="6a99f-140">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
    - <span data-ttu-id="6a99f-141">A jelszó-visszaírással kapcsolatos problémák hibaelhárítási lépéseit a Jelszóvisszaírási hibák [elhárítása című szakaszban láthatja.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="6a99f-141">For more troubleshooting steps for issues with password writeback, see the section [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="6a99f-142">**Nem tudom, hogyan állíthatom alaphelyzetbe egy felhasználó jelszavát**</span><span class="sxs-lookup"><span data-stu-id="6a99f-142">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="6a99f-143">Jelentkezzen be az Azure Portalba megfelelő rendszergazdaként.</span><span class="sxs-lookup"><span data-stu-id="6a99f-143">Sign in to the Azure portal as an appropriate admin.</span></span>
1. <span data-ttu-id="6a99f-144">A Felhasználók és csoportok panelen válassza a **Minden felhasználó lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="6a99f-144">Go to the Users and groups blade, select **All Users**.</span></span>
1. <span data-ttu-id="6a99f-145">Válasszon ki egy felhasználót a listából.</span><span class="sxs-lookup"><span data-stu-id="6a99f-145">Select a user from the list.</span></span>
1. <span data-ttu-id="6a99f-146">A kijelölt felhasználónál válassza az **Áttekintés** lehetőséget, majd a parancssávon kattintson a **Jelszó alaphelyzetbe állítása parancsra.**</span><span class="sxs-lookup"><span data-stu-id="6a99f-146">For the selected user, select **Overview**, and then in the command bar, click **Reset password**.</span></span>
1. <span data-ttu-id="6a99f-147">Kövesse a képernyőn megjelenő utasításokat.</span><span class="sxs-lookup"><span data-stu-id="6a99f-147">Follow the instructions on the screen.</span></span>
    - <span data-ttu-id="6a99f-148">Csak az Azure Portal támogatási jelszavának visszaírásán keresztül végrehajtott visszaállítások.</span><span class="sxs-lookup"><span data-stu-id="6a99f-148">Only resets performed through the Azure portal support password writeback.</span></span>

<span data-ttu-id="6a99f-149">**Alaphelyzetbe állíthatom egy helyszíni felhasználó jelszavát az Office 365 Felügyeleti portálról vagy az Office 365 mobilalkalmazásból, de a felhasználó továbbra sem tud bejelentkezni**</span><span class="sxs-lookup"><span data-stu-id="6a99f-149">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="6a99f-150">Ebben a portálban nem támogatott a jelszó-visszaírás.</span><span class="sxs-lookup"><span data-stu-id="6a99f-150">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="6a99f-151">A felhasználó jelszavának alaphelyzetbe állítása az Azure Portalon – portal.azure.com</span><span class="sxs-lookup"><span data-stu-id="6a99f-151">Reset the user's password again in the Azure portal - portal.azure.com</span></span>

