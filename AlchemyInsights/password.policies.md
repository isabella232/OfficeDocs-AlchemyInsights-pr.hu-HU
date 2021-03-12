---
title: Jelszóházirendek
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 826e266d08aa68c0d4213d8058a0244f404fe965
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744987"
---
# <a name="password-policies"></a><span data-ttu-id="78681-102">Jelszóházirendek</span><span class="sxs-lookup"><span data-stu-id="78681-102">Password policies</span></span>

<span data-ttu-id="78681-103">**Problémát tapasztalok egy felhasználó jelszó-házirend-problémáival**</span><span class="sxs-lookup"><span data-stu-id="78681-103">**I'm having problems with the password policy for a user**</span></span>

- <span data-ttu-id="78681-104">A felhasználók jelszó-házirendjétől függ, hogy a felhasználó csak a felhőben vagy a helyszínen van-e.</span><span class="sxs-lookup"><span data-stu-id="78681-104">The password policy for a user depends on whether the user is cloud only or on-premises.</span></span>
- <span data-ttu-id="78681-105">A csak felhőbeli felhasználóknak a következő cikkben olvasható követelményeknek megfelelő jelszót kell választaniuk: A kizárólag felhőbeli felhasználói fiókokra vonatkozó [jelszó-házirendek](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span><span class="sxs-lookup"><span data-stu-id="78681-105">Cloud only users must choose a password that meets the requirements in this article: [Password policies that only apply to cloud user accounts](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span></span>
- <span data-ttu-id="78681-106">A helyszíni felhasználóknak olyan jelszót kell választaniuk, amely megfelel a helyszíni követelményeknek.</span><span class="sxs-lookup"><span data-stu-id="78681-106">On-premises users must choose a password that meets the on-premises requirements.</span></span> <span data-ttu-id="78681-107">Ha egy helyszíni felhasználó nem tudja beállítani a jelszavát, ellenőrizze a helyszíni követelményeket.</span><span class="sxs-lookup"><span data-stu-id="78681-107">If an on-premises user is unable to set their password, check your on-premises requirements.</span></span>

<span data-ttu-id="78681-108">**Nem tudom, hogyan lehet jelszó lejárati házirendeket beállítani vagy ellenőrizni**</span><span class="sxs-lookup"><span data-stu-id="78681-108">**I don't know how to set or check password expiration policies**</span></span>

- <span data-ttu-id="78681-109">A bérlői felhő felhasználóinak lejárati házirendje a PowerShell használatával beállítható és ellenőrizheti.</span><span class="sxs-lookup"><span data-stu-id="78681-109">You can set and check the expiration policy for cloud users in your tenant by using PowerShell.</span></span> <span data-ttu-id="78681-110">Kövesse a következő cikkben található utasításokat: Jelszó házirendek beállítása vagy [ellenőrzése a PowerShell használatával](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span><span class="sxs-lookup"><span data-stu-id="78681-110">Follow the instructions in this article: [Set or check the password policies by using PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span></span>
- <span data-ttu-id="78681-111">A helyszíni felhasználók jelszó lejárati házirendjére a helyszíni AD-ben van beállítva.</span><span class="sxs-lookup"><span data-stu-id="78681-111">The password expiration policy for on-premises users is set in your on-premises AD.</span></span>

<span data-ttu-id="78681-112">**További hasznos hivatkozások:**</span><span class="sxs-lookup"><span data-stu-id="78681-112">**Other Helpful links:**</span></span>
- [<span data-ttu-id="78681-113">Jelszó-visszaállítás – Első lépések</span><span class="sxs-lookup"><span data-stu-id="78681-113">Getting Started with Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [<span data-ttu-id="78681-114">Rendszergazda által kezdeményezett jelszó-visszaállítás hibaelhárítása</span><span class="sxs-lookup"><span data-stu-id="78681-114">Troubleshoot Administrator-initiated Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
