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
ms.openlocfilehash: 276f6b2212c9d85df726cb46a46dee7828b34c89
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36545170"
---
# <a name="issues-with-mfa"></a>MFA problémái
Néhány dolgot ellenőrizni, ha a felhasználók bejelentkezési többtényezős hitelesítést (MFA) használata nem

1. Az érintett felhasználó Azure Active Directory Portal blokkolhatja. Ez a helyzet, ha hitelesítési kísérletet tesz, hogy az adott felhasználó automatikusan megtagadja. [A Tiltás cikkben leírt lépéseket kövesse.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Ha a felhasználó blokkolásának feloldása nem nyújtott segítséget, vagy nem blokkolja a felhasználó MFA alaphelyzetbe a felhasználó próbálja meg, és ezek azok az igénylés folyamatát újra. [Kövesse a cikkben leírt lépéseket.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Ha az első alkalommal engedélyezett MFA és a felhasználók nem tud bejelentkezni a nem-böngészőkből ügyfelek például az Outlook, Skype, stb, esetleg ADAL (az Active Directory hitelesítési függvénytár) nem engedélyezett a O365 előfizetését. Ebben az esetben kell az Exchange Online Powershell kapcsolódni, és ez a parancsmag futtatásához:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*