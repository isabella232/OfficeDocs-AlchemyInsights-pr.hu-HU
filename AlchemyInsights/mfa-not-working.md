---
title: A MFA problémái
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755133"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="12dfa-102">Az Azure MFA hibáinak elhárítása</span><span class="sxs-lookup"><span data-stu-id="12dfa-102">Issues with Azure MFA</span></span>
<span data-ttu-id="12dfa-103">Van néhány dolog, amit érdemes ellenőrizni, hogy a felhasználók nem tudnak-e bejelentkezni több tényezős hitelesítéssel (MFA)</span><span class="sxs-lookup"><span data-stu-id="12dfa-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="12dfa-104">Lehet, hogy az érintett felhasználó le van tiltva az Azure Active Directory-portálon.</span><span class="sxs-lookup"><span data-stu-id="12dfa-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="12dfa-105">Ha ez a helyzet, akkor a rendszer automatikusan megtagadja a hitelesítési kísérleteket az adott felhasználó számára.</span><span class="sxs-lookup"><span data-stu-id="12dfa-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="12dfa-106">Kérjük, hogy távolítsa el a tiltást a jelen cikkben található lépéseket követve.</span><span class="sxs-lookup"><span data-stu-id="12dfa-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="12dfa-107">Ha a felhasználó feloldása nem segít, vagy a felhasználó nincs letiltva, megpróbálhatja alaphelyzetbe állítani az MFA-t a felhasználó számára, és ismét az igénylési folyamatba kerülnek.</span><span class="sxs-lookup"><span data-stu-id="12dfa-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="12dfa-108">Kérjük, kövesse a jelen cikkben található lépéseket.</span><span class="sxs-lookup"><span data-stu-id="12dfa-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="12dfa-109">Ha először engedélyezte a MFA használatát, és a felhasználók nem tudnak bejelentkezni az olyan nem böngészőkben lévő ügyfeleknek, mint például az Outlook, a Skype, stb., az O365-előfizetésben nincs engedélyezve a ADAL (Active Directory Authentication Library).</span><span class="sxs-lookup"><span data-stu-id="12dfa-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="12dfa-110">Ebben az esetben csatlakoznia kell az Exchange Online Powershellhez, és futtatnia kell a következő parancsmagot:  *Set-OrganizationalSetting-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="12dfa-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>