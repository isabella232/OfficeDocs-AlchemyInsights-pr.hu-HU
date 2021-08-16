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
ms.openlocfilehash: b39c79063c66ea41585c8f9eec372bfac77bc0aa29ded5a5572e06c141b28f80
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098604"
---
# <a name="issues-with-azure-mfa"></a>Az Azure MFA-val kapcsolatos problémák
Van néhány dolog, amit ellenőrizni kell, hogy a felhasználók nem tudnak-e bejelentkezni többtényezős hitelesítéssel (MFA)

1. Előfordulhat, hogy az érintett felhasználó le lesz tiltva a Azure Active Directory portálon. Ebben az esetben a rendszer automatikusan elutasítja az adott felhasználó hitelesítési próbálkozását. [A tiltás feloldásához kövesse a cikkben található lépéseket.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Ha a felhasználó letiltásának feloldása nem segít, vagy ha a felhasználó nem tiltja le, próbálja meg alaphelyzetbe állítani a felhasználó több hitelesítését, és a felhasználó ismét neki is el fog menni a regisztrációs folyamaton. [Kérjük, kövesse a cikkben található lépéseket.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Ha első alkalommal engedélyezi az MFA hitelesítést, és a felhasználói nem tudnak bejelentkezni a nem böngészős ügyfélprogramokkal (például Outlook, Skype stb.), előfordulhat, hogy az ADAL (Active Directory authentication Library) nincs engedélyezve az O365-előfizetésében. Ebben az esetben csatlakoznia kell egy Exchange Online powershellhez, és futtatnia kell a következő parancsmagot: *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*