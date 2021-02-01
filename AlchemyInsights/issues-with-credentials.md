---
title: Hitelesítő adatokkal kapcsolatos problémák
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
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063679"
---
# <a name="issues-with-credentials"></a><span data-ttu-id="7ba52-102">Hitelesítő adatokkal kapcsolatos problémák</span><span class="sxs-lookup"><span data-stu-id="7ba52-102">Issues with credentials</span></span>

<span data-ttu-id="7ba52-103">[A Microsoft identitásplatformja és az OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) ügyfél hitelesítő adatok áramlása azt ismerteti, hogy miként lehet közvetlenül az OAuth 2.0-ügyfél hitelesítő adataival programokat beprogramni.</span><span class="sxs-lookup"><span data-stu-id="7ba52-103">[Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) describes how to program directly against the OAuth 2.0 client credentials grant flow.</span></span>

<span data-ttu-id="7ba52-104">**Hogyan kezelem egy alkalmazás jelszavát vagy tanúsítványának hitelesítő adatait?**</span><span class="sxs-lookup"><span data-stu-id="7ba52-104">**How do I manage an application's password or certificate credentials?**</span></span>

<span data-ttu-id="7ba52-105">Az Azure CLI szolgáltatásban az [ad app](https://docs.microsoft.com/cli/azure/ad/app/credential) hitelesítő adataival törölheti, listálhatja vagy alaphelyzetbe állíthatja egy alkalmazás jelszavát vagy tanúsítványának hitelesítő adatait.</span><span class="sxs-lookup"><span data-stu-id="7ba52-105">In the Azure CLI, you can use [az ad app credential](https://docs.microsoft.com/cli/azure/ad/app/credential) to delete, list, or reset an application's password or certificate credentials.</span></span>

<span data-ttu-id="7ba52-106">**Hogyan állíthatják alaphelyzetbe a felhasználóim a jelszavukat?**</span><span class="sxs-lookup"><span data-stu-id="7ba52-106">**How do my users reset their passwords?**</span></span>

<span data-ttu-id="7ba52-107">A felhasználóknak regisztrálniuk kell [az önkiszolgáló jelszó-visszaállításra,](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) mielőtt alaphelyzetbe állíthatják jelszavukat.</span><span class="sxs-lookup"><span data-stu-id="7ba52-107">Users need to [register for self-service password reset](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) before they can reset their passwords.</span></span> <span data-ttu-id="7ba52-108">Miután regisztrált egy felhasználó, a felhasználó a cikkben található utasításokat követve alaphelyzetbe állíthatja a jelszavát: Állítsa alaphelyzetbe munkahelyi vagy [iskolai jelszavát.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)</span><span class="sxs-lookup"><span data-stu-id="7ba52-108">Once a user has registered, they can follow the instructions in this article to reset their password: [Reset your work or school password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span></span>

<span data-ttu-id="7ba52-109">**Hogyan módosítják a felhasználóim a jelszavukat?**</span><span class="sxs-lookup"><span data-stu-id="7ba52-109">**How do my users change their passwords?**</span></span>

<span data-ttu-id="7ba52-110">A felhasználók a cikkben található lépéseket követve módosíthatjak a jelszavukat: A [jelszó módosítása.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)</span><span class="sxs-lookup"><span data-stu-id="7ba52-110">Users can follow the steps in this article to change their passwords: [How to change your password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span></span>
<span data-ttu-id="7ba52-111">A [kétlépéses ellenőrzés alkalmazásjelszavát is kezelhetik.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)</span><span class="sxs-lookup"><span data-stu-id="7ba52-111">They can also [Manage app passwords for two-step verification](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span></span>

<span data-ttu-id="7ba52-112">**A felhasználó hibaüzenetet kap a jelszavuk módosításakor vagy alaphelyzetbe állításakor**</span><span class="sxs-lookup"><span data-stu-id="7ba52-112">**My user is getting an error when changing or resetting their password**</span></span>

<span data-ttu-id="7ba52-113">Ez a hivatkozás információkat nyújt a felhasználók jelszavának alaphelyzetbe állításakor felmerülő gyakori problémákról: Gyakori problémákról és [megoldásukról](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span><span class="sxs-lookup"><span data-stu-id="7ba52-113">This link will provide information on common problems that can arise when a user is trying to reset their password: [Common problems and their solutions](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span></span>

<span data-ttu-id="7ba52-114">**Probléma adva egy felhasználó jelszavának alaphelyzetbe állítása után**</span><span class="sxs-lookup"><span data-stu-id="7ba52-114">**I'm having a problem resetting a user's password**</span></span>

- <span data-ttu-id="7ba52-115">Győződjön meg arról, hogy jogosult a jelszavak alaphelyzetbe állításra.</span><span class="sxs-lookup"><span data-stu-id="7ba52-115">Make sure you are authorized to reset passwords.</span></span> <span data-ttu-id="7ba52-116">*Csak a globális, a jelszó és a felhasználói rendszergazdák állíthatják alaphelyzetbe a felhasználói jelszavakat.*</span><span class="sxs-lookup"><span data-stu-id="7ba52-116">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="7ba52-117">A globális rendszergazdák más jogosultsággal rendelkező rendszergazdák jelszavát is alaphelyzetbe állíthatják.</span><span class="sxs-lookup"><span data-stu-id="7ba52-117">Global administrators can also reset other privileged administrator's passwords.</span></span>

- <span data-ttu-id="7ba52-118">Győződjön meg arról, hogy megértette a licencelési követelményeket:</span><span class="sxs-lookup"><span data-stu-id="7ba52-118">Make sure you understand the licensing requirements:</span></span>

  - <span data-ttu-id="7ba52-119">A szervezetéhez legalább egy licencnek hozzá kell rendelnie:</span><span class="sxs-lookup"><span data-stu-id="7ba52-119">You must have at least one license assigned in your organization:</span></span>
    - <span data-ttu-id="7ba52-120">**Csak felhőbeli felhasználók** – Bármely Office 365 -ös (O365) fizetős termékváltozat vagy Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="7ba52-120">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="7ba52-121">**Felhőbeli és/vagy helyszíni** felhasználók – Azure AD Premium P1 vagy P2, Enterprise Mobility + Security (EMS) vagy Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="7ba52-121">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="7ba52-122">A licencelési követelményekről az [Azure AD önkiszolgáló jelszó-visszaállítási licenckövetelményei között olvashat bővebben.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="7ba52-122">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span></span>
- <span data-ttu-id="7ba52-123">A felhasználók jelszavának alaphelyzetbe állításához keresse meg a felhasználót az Azure AD-ban.</span><span class="sxs-lookup"><span data-stu-id="7ba52-123">To reset a user's password, find the user in Azure AD.</span></span> <span data-ttu-id="7ba52-124">Ezután kattintson a felhasználó áttekintő paneljének "Jelszó alaphelyzetbe állítása" gombjára.</span><span class="sxs-lookup"><span data-stu-id="7ba52-124">Then, on the overview blade for that user, click the "reset password" button.</span></span>

<span data-ttu-id="7ba52-125">**A jelszó-visszaállítás gomb szürkével kiszürkül**</span><span class="sxs-lookup"><span data-stu-id="7ba52-125">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="7ba52-126">Ön nem jogosult a  felhasználó jelszavának alaphelyzetbe állítania.</span><span class="sxs-lookup"><span data-stu-id="7ba52-126">You are not authorized to reset **this** user's passwords.</span></span> <span data-ttu-id="7ba52-127">*Csak a globális, a jelszó és a felhasználói rendszergazdák állíthatják alaphelyzetbe a felhasználói jelszavakat.*</span><span class="sxs-lookup"><span data-stu-id="7ba52-127">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="7ba52-128">A globális rendszergazdák más jogosultsággal rendelkező rendszergazdák jelszavát is alaphelyzetbe állíthatják.</span><span class="sxs-lookup"><span data-stu-id="7ba52-128">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="7ba52-129">**Nem látom a jelszó-visszaállítási panelt**</span><span class="sxs-lookup"><span data-stu-id="7ba52-129">**I don't see the password reset blade**</span></span>

<span data-ttu-id="7ba52-130">Ön nem jogosult a jelszavak alaphelyzetbe állításra.</span><span class="sxs-lookup"><span data-stu-id="7ba52-130">You are not authorized to reset passwords.</span></span> <span data-ttu-id="7ba52-131">*Csak a globális, a jelszó és a felhasználói rendszergazdák állíthatják alaphelyzetbe a felhasználói jelszavakat.*</span><span class="sxs-lookup"><span data-stu-id="7ba52-131">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="7ba52-132">A globális rendszergazdák más jogosultsággal rendelkező rendszergazdák jelszavát is alaphelyzetbe állíthatják.</span><span class="sxs-lookup"><span data-stu-id="7ba52-132">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="7ba52-133">**Nem látom a helyszíni integrációs panelt a jelszó-visszaállításban**</span><span class="sxs-lookup"><span data-stu-id="7ba52-133">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="7ba52-134">A helyszíni integrációs blade csak hibrid környezetekben jelenik meg – ami azt jelenti, hogy jelszó-visszaírást használ a helyszíni felhasználók jelszavának a módosítása érdekében.</span><span class="sxs-lookup"><span data-stu-id="7ba52-134">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>

- <span data-ttu-id="7ba52-135">Ez a kés nem látható, ha:</span><span class="sxs-lookup"><span data-stu-id="7ba52-135">You do not see this blade if:</span></span>

  - <span data-ttu-id="7ba52-136">Nem jelszó-visszaírást használ</span><span class="sxs-lookup"><span data-stu-id="7ba52-136">You are not using password writeback</span></span>
  - <span data-ttu-id="7ba52-137">Probléma van a jelszó-visszaírás telepítésével/csatlakoztatásával</span><span class="sxs-lookup"><span data-stu-id="7ba52-137">There is a problem with your installation/connectivity of password writeback</span></span>
  - <span data-ttu-id="7ba52-138">Probléma van az Azure AD Connect telepítésével/csatlakoztatásával</span><span class="sxs-lookup"><span data-stu-id="7ba52-138">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
  - <span data-ttu-id="7ba52-139">A jelszóvisszaírással kapcsolatos hibák hibaelhárítási lépéseit a Jelszóvisszaírási hibák [elhárítása témakörben láthatja.](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="7ba52-139">For more troubleshooting steps for issues with password writeback, see [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span></span>

<span data-ttu-id="7ba52-140">**Nem tudom, hogyan állíthatom alaphelyzetbe egy felhasználó jelszavát**</span><span class="sxs-lookup"><span data-stu-id="7ba52-140">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="7ba52-141">Jelentkezzen be az Azure Portalba megfelelő rendszergazdaként.</span><span class="sxs-lookup"><span data-stu-id="7ba52-141">Sign in to the Azure portal as an appropriate admin.</span></span>
2. <span data-ttu-id="7ba52-142">A Felhasználók és **csoportok panelen** válassza a **Minden felhasználó lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="7ba52-142">Go to the **Users and groups** blade, select **All Users**.</span></span>
3. <span data-ttu-id="7ba52-143">Jelöljön ki egy felhasználót a listából.</span><span class="sxs-lookup"><span data-stu-id="7ba52-143">Select a user from the list.</span></span>
4. <span data-ttu-id="7ba52-144">A kijelölt felhasználónál válassza az **Áttekintés** lehetőséget, majd a parancssávon válassza a **Jelszó alaphelyzetbe állítása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="7ba52-144">For the selected user, select **Overview**, and then in the command bar, select **Reset password**.</span></span>
5. <span data-ttu-id="7ba52-145">Válassza a **Jelszó alaphelyzetbe állítása** gombot, és kövesse a képernyőn megjelenő utasításokat.</span><span class="sxs-lookup"><span data-stu-id="7ba52-145">Select the **Reset password** button and follow the instructions on the screen.</span></span>
    - <span data-ttu-id="7ba52-146">Csak az Azure **Portal** támogatási jelszavának visszaírásán keresztül végrehajtott visszaállítások.</span><span class="sxs-lookup"><span data-stu-id="7ba52-146">Only resets performed through the **Azure portal** support password writeback.</span></span>

<span data-ttu-id="7ba52-147">**Alaphelyzetbe állíthatom egy helyszíni felhasználó jelszavát az Office 365 Felügyeleti portálról vagy az Office 365 mobilalkalmazásból, de a felhasználó továbbra sem tud bejelentkezni**</span><span class="sxs-lookup"><span data-stu-id="7ba52-147">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="7ba52-148">Ebben a portálban nem támogatott a jelszó-visszaírás.</span><span class="sxs-lookup"><span data-stu-id="7ba52-148">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="7ba52-149">Állítsa alaphelyzetbe ismét a felhasználó jelszavát az Azure Portalon.</span><span class="sxs-lookup"><span data-stu-id="7ba52-149">Reset the user's password again in the Azure portal.</span></span>
