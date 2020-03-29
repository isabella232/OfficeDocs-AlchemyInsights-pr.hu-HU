---
title: Nem lehet bejelentkezni a Teamsbe az autologon.microsoftazuread-sso.com:443 hiba miatt
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932043"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>Nem lehet bejelentkezni a Teamsbe az autologon.microsoftazuread-sso dot com:443 hiba miatt

Ha közvetlen egyszeri bejelentkezés engedélyezett az Office 365-ös hitelesítésként, előfordulhat, hogy az „autologon.microsoftazuread-sso.com” URL-címet hozzá kell adni az intranetes helyekhez.  Ha már korábban hozzáadta a megbízható helyekhez, és közvetlen egyszeri bejelentkezést használ, el kell távolítania a megbízható helyek közül.

Tanulmányozza a [közvetlen egyszeri bejelentkezés hibaelhárítási ellenőrzőlistáját](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).

Ezeket a lépéseket követve vegyen fel URL-címeket az intranetes helyek listájára:

1. A **Start** gombra kattintva nyissa meg az Internet Explorert. A keresőmezőbe írja be az Internet Explorer nevet, majd a találatok listájában kattintson az **Internet Explorer** elemre.
2. Válassza az **Eszközök** menü **Internetbeállítások** parancsát.
3. Kattintson a **Biztonság** fülre.
4. Ezután kattintson a **Helyi intranet** ikonra, majd a **Helyek** gombra, végül a **Speciális** gombra.
5. Adja meg a webhely URL-címét, és kattintson a **Hozzáadás** gombra.
6. Amikor elkészült, kattintson a **Bezárás** gombra.

További információt a [közvetlen egyszeri bejelentkezés Office 365-höz való telepítésének dokumentációjában](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) talál (a 3. lépés az URL-cím intranetes helyekhez való hozzáadásának házirendalapú eljárását tartalmazza).
