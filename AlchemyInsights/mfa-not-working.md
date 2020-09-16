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
# <a name="issues-with-azure-mfa"></a>Az Azure MFA hibáinak elhárítása
Van néhány dolog, amit érdemes ellenőrizni, hogy a felhasználók nem tudnak-e bejelentkezni több tényezős hitelesítéssel (MFA)

1. Lehet, hogy az érintett felhasználó le van tiltva az Azure Active Directory-portálon. Ha ez a helyzet, akkor a rendszer automatikusan megtagadja a hitelesítési kísérleteket az adott felhasználó számára. [Kérjük, hogy távolítsa el a tiltást a jelen cikkben található lépéseket követve.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Ha a felhasználó feloldása nem segít, vagy a felhasználó nincs letiltva, megpróbálhatja alaphelyzetbe állítani az MFA-t a felhasználó számára, és ismét az igénylési folyamatba kerülnek. [Kérjük, kövesse a jelen cikkben található lépéseket.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Ha először engedélyezte a MFA használatát, és a felhasználók nem tudnak bejelentkezni az olyan nem böngészőkben lévő ügyfeleknek, mint például az Outlook, a Skype, stb., az O365-előfizetésben nincs engedélyezve a ADAL (Active Directory Authentication Library). Ebben az esetben csatlakoznia kell az Exchange Online Powershellhez, és futtatnia kell a következő parancsmagot:  *Set-OrganizationalSetting-OAuth2ClientProfileEnabled: $true*