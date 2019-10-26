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
ms.openlocfilehash: 276f6b2212c9d85df726cb46a46dee7828b34c89
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/25/2019
ms.locfileid: "36545170"
---
# <a name="issues-with-mfa"></a>Kérdések az MFA-val kapcsolatban
Vannak egy pár dolog-hoz ellenőriz ha használók nem tud logika használ multi--tényező hitelesítés (MFA)

1. Lehetséges, hogy a rendszer letiltotta az érintett felhasználót a Azure Active Directory Portal webhelyen. Ebben az esetben a rendszer automatikusan megtagadja a hitelesítési kísérleteket az adott felhasználóra vonatkozóan. [A letiltáshoz kövesse az ebben a cikkben leírt lépéseket.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Ha feloldását a felhasználó nem segít, vagy a felhasználó nem blokkolja tudod megpróbál-hoz orrgazdaság MFA a felhasználó számára, és mennek keresztül az igénylési folyamat újra. [Kérjük, kövesse a cikkben leírt lépéseket.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Ha ez a először Ön lehetővé tett MFA és-a használók van képtelen-hoz logika-hoz nem-legel ügyfelek mint Kilátás, Skype, stb, talán ADAL (aktivál címtár hitelesítés könyvtár) van nem lehetővé tett-ra-a O365 aláírás. Ebben az esetben az Exchange Online PowerShell eszközzel kell kapcsolódnia, és futtatni kell ezt a parancsmagot:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*