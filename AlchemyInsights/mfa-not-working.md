---
title: Kérdések az MFA-val kapcsolatban
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
ms.openlocfilehash: a415116b9ba437cb13426896119cd1b40d9ab491
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768839"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="94466-102">Kérdések Azure MFA</span><span class="sxs-lookup"><span data-stu-id="94466-102">Issues with Azure MFA</span></span>
<span data-ttu-id="94466-103">Vannak egy pár dolog-hoz ellenőriz ha használók nem tud fatörzs-ban használ multi--tényező hitelesítés (MFA)</span><span class="sxs-lookup"><span data-stu-id="94466-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="94466-104">Lehetséges, hogy a rendszer letiltotta az érintett felhasználót a Azure Active Directory Portal webhelyen.</span><span class="sxs-lookup"><span data-stu-id="94466-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="94466-105">Ebben az esetben a rendszer automatikusan megtagadja a hitelesítési kísérleteket az adott felhasználóra vonatkozóan.</span><span class="sxs-lookup"><span data-stu-id="94466-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="94466-106">A letiltáshoz kövesse az ebben a cikkben leírt lépéseket.</span><span class="sxs-lookup"><span data-stu-id="94466-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="94466-107">Ha feloldását a felhasználó nem segít, vagy a felhasználó nem blokkolja tudod megpróbál-hoz orrgazdaság MFA a felhasználó számára, és mennek keresztül az igénylési folyamat újra.</span><span class="sxs-lookup"><span data-stu-id="94466-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="94466-108">Kérjük, kövesse a cikkben leírt lépéseket.</span><span class="sxs-lookup"><span data-stu-id="94466-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="94466-109">Ha ez a először Ön lehetővé tett MFA és-a használók van képtelen-hoz logika-hoz nem-legel ügyfelek mint Kilátás, Skype, stb, talán ADAL (aktivál címtár hitelesítés könyvtár) van nem lehetővé tett-ra-a O365 aláírás.</span><span class="sxs-lookup"><span data-stu-id="94466-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="94466-110">Ebben az esetben az Exchange Online PowerShell eszközzel kell kapcsolódnia, és futtatni kell ezt a parancsmagot:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="94466-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>