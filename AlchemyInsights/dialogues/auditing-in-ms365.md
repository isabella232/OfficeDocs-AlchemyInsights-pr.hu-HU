---
title: Naplózás a Microsoft 365-ben
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
ms.openlocfilehash: c07981bfae40d74deb1a2f143ce51da69b51a69f
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429649"
---
# <a name="auditing-in-microsoft-365"></a>Naplózás a Microsoft 365-ben

Íme néhány dolog, amit érdemes tudnia a Microsoft 365 naplózásával kapcsolatban:

1. Az Exchange-rendszergazdai tevékenységek naplózása alapértelmezés szerint meg van jelölve.
1. Folyamatban van a postaláda-naplózás alapértelmezés szerint bekapcsolása az összes felhasználónál. További információért kattintson [ide.](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Exchange-Mailbox-Auditing-will-be-enabled-by-default/ba-p/215171) Addig is, ha azt szeretné, hogy az utasításokat manuálisan engedélyezze egy személy vagy egy teljes szervezet számára, válassza az alábbi Postaláda-naplózás bekapcsolása gombot.
1. A Microsoft 365-csoportok postaládái és a nyilvánosmappa-postaládák nem támogatják a naplózást.
1. A SharePoint/OneDrive esetén nincs szükség további konfigurációra a naplózás engedélyezett beállításához. A naplóban végzett tevékenységekről a következő cikkből olvashat:
    1. [Fájltevékenységek](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#file-and-page-activities)
    1. [Mappatevékenységek](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    1. [Megosztási és hozzáférési tevékenységek.](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
1. A szolgáltatás szerint naplóolt tevékenységek listáját a Naplós [tevékenységek között láthatja.](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities)
