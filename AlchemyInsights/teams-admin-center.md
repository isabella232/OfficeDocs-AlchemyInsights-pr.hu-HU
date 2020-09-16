---
title: Teams Felügyeleti központ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: bb0d757aab05132ff7169ce75009d7012b9a836c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670366"
---
# <a name="teams-admin-center"></a>Teams Felügyeleti központ

Megtudhatja, hogyan kezelheti a Teams alkalmazást a [Teams Felügyeleti központtal](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Ha nem tudja elérni a Teams Felügyeleti központot, ellenőrizze az alábbiakat:

- Győződjön meg arról, hogy engedélyezte a megfelelő [IP-címeket és URL-címeket az Office 365-höz](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) a peremhálózati eszközökön (tűzfalon stb.), illetve a helyi számítógépen beállított tűzfalszabályokban.
- Győződjön meg arról, hogy a Teams felügyeleti portál eléréséhez használt bejelentkezési név megegyezik a [Microsoft 365 felügyeleti portálon](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) megadott felhasználónevével.

Ha nem jelennek meg felhasználók a Teams Felügyeleti központban, ellenőrizze az alábbiakat:

- Létrehozott felhasználókat, vagy kiosztott licenceket az elmúlt 24 órában? Kérjük, várjon legalább 24 órát, mielőtt támogatási jegyet nyitna.
- Ellenőrizze: megfelelő licenceket rendelt hozzá a felhasználókhoz?
- Ha helyszíni Active Directory-címtárral rendelkezik, győződjön meg arról, hogy [az msRTCSIP-PrimaryUserAddress vagy a SIP-cím értéke a helyi Active Directory-címtárban a ProxyAddresses mezőben látható, és a formátum megegyezik](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) a SIP: felhasználó**felhasználónevével** a [Microsoft 365 felügyeleti központjában](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Ha meg kívánja őrizni a Skype vállalati verzió kiszolgálójának telepítési példányát, és a helyszíni és online otthoni felhasználóknak is elérhetővé szeretné tenni a felhasználókat, tegye a következőket: a **hibrid beállítás beállítása a Teams és a Skype vállalati online** verzióhoz a Skype vállalati verzió kiszolgálójának Vezérlőpultján, és helyezze át a felhasználókat az interneten.
