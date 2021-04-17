---
title: Teams Felügyeleti központ
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: 4a3a0796cedd81919066d870c5ca99fe2e978cf8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826381"
---
# <a name="teams-admin-center"></a>Teams Felügyeleti központ

Megtudhatja, hogyan kezelheti a Teams alkalmazást a [Teams Felügyeleti központtal](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Ha nem tudja elérni a Teams Felügyeleti központot, ellenőrizze az alábbiakat:

- Győződjön meg arról, hogy engedélyezte a megfelelő [IP-címeket és URL-címeket az Office 365-höz](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) a peremhálózati eszközökön (tűzfalon stb.), illetve a helyi számítógépen beállított tűzfalszabályokban.
- Győződjön meg arról, hogy a Teams felügyeleti portál eléréséhez használt bejelentkezési név megegyezik a [Microsoft 365 felügyeleti portálon](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) megadott felhasználónevével.

Ha nem jelennek meg felhasználók a Teams Felügyeleti központban, ellenőrizze az alábbiakat:

- Létrehozott felhasználókat, vagy kiosztott licenceket az elmúlt 24 órában? Kérjük, várjon legalább 24 órát, mielőtt támogatási jegyet nyitna.
- Ellenőrizze: megfelelő licenceket rendelt hozzá a felhasználókhoz?
- Ha helyszíni Active Directoryt használ, ellenőrizze, hogy az [msRTCSIP-PrimaryUserAddress](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) érték vagy a helyi Active Directory ProxyAddresses mezőjében lévő SIP-cím egyedi-e, és a formátum megegyezik a sip:**A** felhasználó felhasználóneve a [Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)Felügyeleti központban.
- Ha meg szeretné tartani a Skype Vállalati kiszolgáló telepítését, és szeretné, hogy a felhasználók a helyszínen és online környezetben is üzemelnek, kövesse a Skype Vállalati kiszolgáló Vezérlőpultjának **"Hibrid** környezet beállítása a Teams és a Skype Vállalati online verzióval" című útmutatóját, és helyezze át a felhasználókat online.
