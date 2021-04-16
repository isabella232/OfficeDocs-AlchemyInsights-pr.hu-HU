---
title: Az MFA-val kapcsolatos problémák
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810486"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="d5033-102">Az Azure MFA-val kapcsolatos problémák</span><span class="sxs-lookup"><span data-stu-id="d5033-102">Issues with Azure MFA</span></span>
<span data-ttu-id="d5033-103">Van néhány dolog, amit ellenőrizni kell, hogy a felhasználók nem tudnak-e bejelentkezni többtényezős hitelesítéssel (MFA)</span><span class="sxs-lookup"><span data-stu-id="d5033-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="d5033-104">Előfordulhat, hogy az érintett felhasználó le van tiltva az Azure Active Directory portálon.</span><span class="sxs-lookup"><span data-stu-id="d5033-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="d5033-105">Ebben az esetben a rendszer automatikusan elutasítja az adott felhasználó hitelesítési próbálkozását.</span><span class="sxs-lookup"><span data-stu-id="d5033-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="d5033-106">A tiltás feloldásához kövesse a cikkben található lépéseket.</span><span class="sxs-lookup"><span data-stu-id="d5033-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="d5033-107">Ha a felhasználó letiltásának feloldása nem segít, vagy ha a felhasználó nem tiltja le, próbálja meg alaphelyzetbe állítani a felhasználó több hitelesítését, és a felhasználó ismét neki is el fog menni a regisztrációs folyamaton.</span><span class="sxs-lookup"><span data-stu-id="d5033-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="d5033-108">Kérjük, kövesse a cikkben található lépéseket.</span><span class="sxs-lookup"><span data-stu-id="d5033-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="d5033-109">Ha első alkalommal engedélyezi az MFA hitelesítést, és a felhasználói nem tudnak bejelentkezni a nem böngészős ügyfélprogramokkal , például az Outlookkal, a Skype-pal stb., előfordulhat, hogy az ADAL (Active Directory authentication Library) nincs engedélyezve az O365-előfizetésében.</span><span class="sxs-lookup"><span data-stu-id="d5033-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="d5033-110">Ebben az esetben csatlakoznia kell az Exchange Online Powershellhez, és futtatnia kell a következő parancsmagot:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span><span class="sxs-lookup"><span data-stu-id="d5033-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>