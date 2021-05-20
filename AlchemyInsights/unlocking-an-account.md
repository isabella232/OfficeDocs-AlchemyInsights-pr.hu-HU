---
title: Fiókzárolás feloldása
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002449"
- "4748"
ms.openlocfilehash: cf2431cb49902b3f7625ab96bc6d4e2121e51fdd
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544146"
---
# <a name="unlocking-an-account"></a><span data-ttu-id="61656-102">Fiókzárolás feloldása</span><span class="sxs-lookup"><span data-stu-id="61656-102">Unlocking an account</span></span>

<span data-ttu-id="61656-103">Előfordulhat, hogy a Microsoft 365 kizár felhasználókat hibás jelszóval történő többszöri belépési kísérlet vagy egyéb problémák miatt.</span><span class="sxs-lookup"><span data-stu-id="61656-103">It's possible users are locked out of Microsoft 365 due to bad password attempts or other compromises.</span></span> <span data-ttu-id="61656-104">Az alábbi lépésekkel **segíthet a felhasználóknak visszajelentkezni a Microsoft 365-be, mielőtt támogatási kérést küldene**.</span><span class="sxs-lookup"><span data-stu-id="61656-104">To help users sign back in to Microsoft 365, **you can attempt the following steps before opening a Support Request**.</span></span> 

<span data-ttu-id="61656-105">**E-mailek küldése korlátozva**</span><span class="sxs-lookup"><span data-stu-id="61656-105">**Email Restricted**</span></span>

<span data-ttu-id="61656-106">Ha az egyik felhasználója számára korlátozva van az e-mailek küldése, rendszergazdaként [Ön is feloldhatja a fiók tiltását](/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam).</span><span class="sxs-lookup"><span data-stu-id="61656-106">As an admin, if one of your users is restricted from sending email, you can [unblock the account yourself](/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam).</span></span> <span data-ttu-id="61656-107">A felhasználó a korlátozás eltávolítása után egy órán belül újból tud majd e-mailt küldeni.</span><span class="sxs-lookup"><span data-stu-id="61656-107">The user will be able to send email within an hour after removing the restriction.</span></span>

<span data-ttu-id="61656-108">**Felhasználói jelszó alaphelyzetbe állítása**</span><span class="sxs-lookup"><span data-stu-id="61656-108">**Reset the User Password**</span></span>

1. <span data-ttu-id="61656-109">A felügyeleti központban válassza a **Felhasználók > [Aktív felhasználók](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="61656-109">In the admin center, go to **Users > [Active Users](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)**.</span></span>

2. <span data-ttu-id="61656-110">Jelölje ki a felhasználót, majd kattintson a **Jelszó alaphelyzetbe állítása** elemre.</span><span class="sxs-lookup"><span data-stu-id="61656-110">Select the user and click **Reset Password**.</span></span>

<span data-ttu-id="61656-111">**Gondoskodjon arról, hogy a felhasználó bejelentkezhessen**</span><span class="sxs-lookup"><span data-stu-id="61656-111">**Make sure the user is allowed to sign in**</span></span>

1. <span data-ttu-id="61656-112">A felügyeleti központban válassza a **Felhasználók > [Aktív felhasználók](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="61656-112">In the admin center, go to **Users > [Active Users](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)**.</span></span>

2. <span data-ttu-id="61656-113">Jelölje ki a felhasználót, és kattintson a három pontra (további műveletek), majd a Bejelentkezési **állapot szerkesztése elemre.**</span><span class="sxs-lookup"><span data-stu-id="61656-113">Select the user and click the three dots (more actions), then click **Edit sign-in status**.</span></span>

<span data-ttu-id="61656-114">A jelszavak alaphelyzetbe állításával kapcsolatos további esetekért (beleértve az önkiszolgáló jelszó-visszaállítást is) lásd: [Jelszavak alaphelyzetbe állítása az eszközök a többszöri kísérlet az online fizetés kivitelezésére Microsoft 365 Vállalati verzióban](/microsoft-365/admin/add-users/reset-passwords).</span><span class="sxs-lookup"><span data-stu-id="61656-114">For more password reset scenarios, including Self-Service Password Reset, see [Reset Microsoft 365 for multiple-attempts-to-charge-online-payment-instrumentsbusiness passwords](/microsoft-365/admin/add-users/reset-passwords).</span></span>

<span data-ttu-id="61656-115">A szolgáltatás megakadályozza, hogy a felhasználó e-mailt küldjön egy sérült fiókra és/vagy kimenő levélszemétre utaló bizonyíték észlelése után.</span><span class="sxs-lookup"><span data-stu-id="61656-115">The service prevents a user from sending email after detecting evidence of a compromised account and/or outbound spam.</span></span> <span data-ttu-id="61656-116">Megelőzésképpen végezze el a [Teendők Microsoft 365-ös felhasználói e-mail-fiók feltörése esetén](/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account) című cikkben ismertetett lépéseket.</span><span class="sxs-lookup"><span data-stu-id="61656-116">As a precaution, follow the steps in [Responding to a Compromised Email Account in Microsoft 365](/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account) for the user.</span></span>
