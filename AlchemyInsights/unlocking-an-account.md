---
title: Fiókzárolás feloldása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002449"
- "4748"
ms.openlocfilehash: 3d32123f757a727e1f6ef04270152e276cf803fa
ms.sourcegitcommit: cead49883943b0eb413f8cf4be617a32b5099cb6
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/24/2020
ms.locfileid: "43799053"
---
# <a name="unlocking-an-account"></a><span data-ttu-id="f2711-102">Fiókzárolás feloldása</span><span class="sxs-lookup"><span data-stu-id="f2711-102">Unlocking an account</span></span>

<span data-ttu-id="f2711-103">Előfordulhat, hogy a Microsoft 365 kizár felhasználókat hibás jelszóval történő többszöri belépési kísérlet vagy egyéb problémák miatt.</span><span class="sxs-lookup"><span data-stu-id="f2711-103">It's possible users are locked out of Microsoft 365 due to bad password attempts or other compromises.</span></span> <span data-ttu-id="f2711-104">Az alábbi lépésekkel **segíthet a felhasználóknak visszajelentkezni a Microsoft 365-be, mielőtt támogatási kérést küldene**.</span><span class="sxs-lookup"><span data-stu-id="f2711-104">To help users sign back in to Microsoft 365, **you can attempt the following steps before opening a Support Request**.</span></span> 

<span data-ttu-id="f2711-105">**E-mailek küldése korlátozva**</span><span class="sxs-lookup"><span data-stu-id="f2711-105">**Email Restricted**</span></span>

<span data-ttu-id="f2711-106">Ha az egyik felhasználója számára korlátozva van az e-mailek küldése, rendszergazdaként [Ön is feloldhatja a fiók tiltását](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam).</span><span class="sxs-lookup"><span data-stu-id="f2711-106">As an admin, if one of your users is restricted from sending email, you can [unblock the account yourself](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam).</span></span> <span data-ttu-id="f2711-107">A felhasználó a korlátozás eltávolítása után egy órán belül újból tud majd e-mailt küldeni.</span><span class="sxs-lookup"><span data-stu-id="f2711-107">The user will be able to send email within an hour after removing the restriction.</span></span>

<span data-ttu-id="f2711-108">**Felhasználói jelszó alaphelyzetbe állítása**</span><span class="sxs-lookup"><span data-stu-id="f2711-108">**Reset the User Password**</span></span>

1. <span data-ttu-id="f2711-109">A felügyeleti központban válassza a **Felhasználók > [Aktív felhasználók](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="f2711-109">In the admin center, go to **Users > [Active Users](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)**.</span></span>

2. <span data-ttu-id="f2711-110">Jelölje ki a felhasználót, majd kattintson a **Jelszó alaphelyzetbe állítása** elemre.</span><span class="sxs-lookup"><span data-stu-id="f2711-110">Select the user and click **Reset Password**.</span></span>

<span data-ttu-id="f2711-111">**Gondoskodjon arról, hogy a felhasználó bejelentkezhessen**</span><span class="sxs-lookup"><span data-stu-id="f2711-111">**Make sure the user is allowed to sign in**</span></span>

1. <span data-ttu-id="f2711-112">A felügyeleti központban válassza a **Felhasználók > [Aktív felhasználók](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="f2711-112">In the admin center, go to **Users > [Active Users](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)**.</span></span>

2. <span data-ttu-id="f2711-113">Jelölje ki a felhasználót, és kattintson a **További műveletek (...)** elemre, majd a **Bejelentkezési állapot szerkesztése** lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="f2711-113">Select the user and click **More Actions (...)**; then click **Edit sign-in status**.</span></span>

<span data-ttu-id="f2711-114">A jelszavak alaphelyzetbe állításával kapcsolatos további esetekért (beleértve az önkiszolgáló jelszó-visszaállítást is) lásd: [Jelszavak alaphelyzetbe állítása az eszközök a többszöri kísérlet az online fizetés kivitelezésére Microsoft 365 Vállalati verzióban](https://docs.microsoft.com/microsoft-365/admin/add-users/reset-passwords?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="f2711-114">For more password reset scenarios, including Self-Service Password Reset, see [Reset Microsoft 365 for multiple-attempts-to-charge-online-payment-instrumentsbusiness passwords](https://docs.microsoft.com/microsoft-365/admin/add-users/reset-passwords?view=o365-worldwide).</span></span>

<span data-ttu-id="f2711-115">A szolgáltatás megakadályozza, hogy a felhasználó e-mailt küldjön egy sérült fiókra és/vagy kimenő levélszemétre utaló bizonyíték észlelése után.</span><span class="sxs-lookup"><span data-stu-id="f2711-115">The service prevents a user from sending email after detecting evidence of a compromised account and/or outbound spam.</span></span> <span data-ttu-id="f2711-116">Megelőzésképpen végezze el a [Teendők Microsoft 365-ös felhasználói e-mail-fiók feltörése esetén](https://docs.microsoft.com/office365/securitycompliance/responding-to-a-compromised-email-account) című cikkben ismertetett lépéseket.</span><span class="sxs-lookup"><span data-stu-id="f2711-116">As a precaution, follow the steps in [Responding to a Compromised Email Account in Microsoft 365](https://docs.microsoft.com/office365/securitycompliance/responding-to-a-compromised-email-account) for the user.</span></span>
