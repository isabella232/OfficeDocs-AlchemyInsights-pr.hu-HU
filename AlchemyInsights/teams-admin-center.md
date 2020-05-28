---
title: Teams Felügyeleti központ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: d504a26ee6532ec291eae797b1c81d86a05414b0
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354090"
---
# <a name="teams-admin-center"></a>Teams Felügyeleti központ

Megtudhatja, hogyan kezelheti a Teams alkalmazást a [Teams Felügyeleti központtal](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Ha nem tudja elérni a Teams Felügyeleti központot, ellenőrizze az alábbiakat:

- Győződjön meg arról, hogy engedélyezte a megfelelő [IP-címeket és URL-címeket az Office 365-höz](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) a peremhálózati eszközökön (tűzfalon stb.), illetve a helyi számítógépen beállított tűzfalszabályokban.
- Győződjön meg arról, hogy a Teams felügyeleti portál eléréséhez használt bejelentkezési név megegyezik a [Microsoft 365 felügyeleti portálon](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) megadott felhasználónevével.

Ha nem jelennek meg felhasználók a Teams Felügyeleti központban, ellenőrizze az alábbiakat:

- Létrehozott felhasználókat, vagy kiosztott licenceket az elmúlt 24 órában? Kérjük, várjon legalább 24 órát, mielőtt támogatási jegyet nyitna.
- Ellenőrizze: megfelelő licenceket rendelt hozzá a felhasználókhoz?
- Ha rendelkezik helyszíni Active Directoryval, ellenőrizze, hogy [az msRTCSIP-PrimaryUserAddress vagy a helyi Active Directory ProxyAddresses mezőjében szereplő SIP-cím értéke egyedi-e, és a formátum megegyezik a](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** (Felhasználó neve a [Microsoft 365 felügyeleti központból)](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)mezőben.
- Ha meg kívánja tartani a Skype Vállalati kiszolgáló központi telepítését, és a felhasználókat a helyszínen és az Online szolgáltatásban szeretné elhelyezni: kövesse a Skype Vállalati kiszolgáló vezérlőpultján található "Hibrid beállítása a Teamsszel és a **Skype Vállalati online verzióval"** című részt, és helyezze át a felhasználók online állapotát.
