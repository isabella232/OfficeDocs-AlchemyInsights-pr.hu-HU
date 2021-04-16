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
# <a name="issues-with-azure-mfa"></a>Az Azure MFA-val kapcsolatos problémák
Van néhány dolog, amit ellenőrizni kell, hogy a felhasználók nem tudnak-e bejelentkezni többtényezős hitelesítéssel (MFA)

1. Előfordulhat, hogy az érintett felhasználó le van tiltva az Azure Active Directory portálon. Ebben az esetben a rendszer automatikusan elutasítja az adott felhasználó hitelesítési próbálkozását. [A tiltás feloldásához kövesse a cikkben található lépéseket.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Ha a felhasználó letiltásának feloldása nem segít, vagy ha a felhasználó nem tiltja le, próbálja meg alaphelyzetbe állítani a felhasználó több hitelesítését, és a felhasználó ismét neki is el fog menni a regisztrációs folyamaton. [Kérjük, kövesse a cikkben található lépéseket.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Ha első alkalommal engedélyezi az MFA hitelesítést, és a felhasználói nem tudnak bejelentkezni a nem böngészős ügyfélprogramokkal , például az Outlookkal, a Skype-pal stb., előfordulhat, hogy az ADAL (Active Directory authentication Library) nincs engedélyezve az O365-előfizetésében. Ebben az esetben csatlakoznia kell az Exchange Online Powershellhez, és futtatnia kell a következő parancsmagot:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*