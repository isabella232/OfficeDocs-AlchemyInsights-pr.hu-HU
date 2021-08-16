---
title: Naplózás a Microsoft 365
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: a5acd322186f8f4b7734f8541877a642a553288e10b3c122e4f276b9bb611308
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988975"
---
# <a name="auditing-in-microsoft-365"></a>Naplózás a Microsoft 365

Íme néhány dolog, amit érdemes tudnia a naplózásról a Microsoft 365:

1. Exchange a rendszergazdai tevékenységek naplózása alapértelmezés szerint meg van jelölve.
1. Folyamatban van a postaláda-naplózás alapértelmezés szerinti bekapcsolása az összes felhasználó számára. További információért kattintson [ide.](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Exchange-Mailbox-Auditing-will-be-enabled-by-default/ba-p/215171) Addig is, ha azt szeretné, hogy egy személy vagy egy teljes szervezet számára manuálisan engedélyezze az utasításokat, válassza az alábbi Postaláda-naplózás engedélyezése gombot.
1. Microsoft 365 A csoport- és a nyilvánosmappa-postaládák nem támogatják a naplózást.
1. A SharePoint/OneDrive nincs szükség további konfigurációra az engedélyezett naplózáshoz. Az auditált tevékenységekről a következő cikkből olvashat:
    1. [Fájltevékenységek](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#file-and-page-activities)
    1. [Mappatevékenységek](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    1. [Megosztási és hozzáférési tevékenységek.](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
1. Az összes naplóolt tevékenység szolgáltatás szerint való listáját a [Naplós tevékenységek listában láthatja.](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities)
