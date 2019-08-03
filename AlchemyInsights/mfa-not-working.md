---
title: MFA problémái
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2e79040c249b7825b964a19c51bcc42e5a6afb3f
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/26/2019
ms.locfileid: "35250167"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="cb272-102">MFA problémái</span><span class="sxs-lookup"><span data-stu-id="cb272-102">Issues with MFA</span></span>
<span data-ttu-id="cb272-103">Néhány dolgot ellenőrizni, ha a felhasználók bejelentkezési többtényezős hitelesítést (MFA) használata nem</span><span class="sxs-lookup"><span data-stu-id="cb272-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="cb272-104">Az érintett felhasználó Azure Active Directory Portal blokkolhatja.</span><span class="sxs-lookup"><span data-stu-id="cb272-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="cb272-105">Ez a helyzet, ha hitelesítési kísérletet tesz, hogy az adott felhasználó automatikusan megtagadja.</span><span class="sxs-lookup"><span data-stu-id="cb272-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="cb272-106">A Tiltás cikkben leírt lépéseket kövesse.</span><span class="sxs-lookup"><span data-stu-id="cb272-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="cb272-107">Ha a felhasználó blokkolásának feloldása nem nyújtott segítséget, vagy nem blokkolja a felhasználó MFA alaphelyzetbe a felhasználó próbálja meg, és ezek azok az igénylés folyamatát újra.</span><span class="sxs-lookup"><span data-stu-id="cb272-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="cb272-108">Kövesse a cikkben leírt lépéseket.</span><span class="sxs-lookup"><span data-stu-id="cb272-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="cb272-109">Ha az első alkalommal engedélyezett MFA és a felhasználók nem tud bejelentkezni a nem-böngészőkből ügyfelek például az Outlook, Skype, stb, esetleg ADAL (az Active Directory hitelesítési függvénytár) nem engedélyezett a O365 előfizetését.</span><span class="sxs-lookup"><span data-stu-id="cb272-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="cb272-110">Ebben az esetben kell az Exchange Online Powershell kapcsolódni, és ez a parancsmag futtatásához:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="cb272-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>