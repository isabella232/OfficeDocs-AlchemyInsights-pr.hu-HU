---
title: A Microsoft névkiszolgálóiról való visszaváltás a saját DNS-rekordok kezelésére
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13988"
- "14"
ms.openlocfilehash: a228bcda1220011ab994de7aa70f19ea092e2142
ms.sourcegitcommit: e9e282be4997b0ee95f1ff4491e0943f8fc52444
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506605"
---
# <a name="changing-from-microsoft-nameservers-back-to-managing-your-own-dns-records"></a>A Microsoft névkiszolgálóiról való visszaváltás a saját DNS-rekordok kezelésére

Korábban módosította a névrekordokat úgy, hogy a Microsoftra (ns1.bdm.microsoftonline.com) mutasson, de most úgy döntött, hogy saját maga kezeli a DNS-rekordjait:

A tartományregisztráló webhelyén módosítsa a névkiszolgálót a tartományregisztrálójára vagy a korábbi beállításra. De ha bizonytalan, lépjen kapcsolatba a tartományregisztrálója támogatási szolgálatával. Vegye figyelembe, hogy a névkiszolgáló-módosítások propagálása akár 48 órát is igénybe is vehet. 

1. A Microsoft 365 felügyeleti portálon válassza a **Gépház** Domains (Tartományok) lehetőséget, jelölje be a tartomány melletti jelölőnégyzetet, és válassza a  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains)DNS **kezelése lehetőséget.** 

2. A varázslóban válassza a **Saját DNS-rekordok hozzáadása lehetőséget, és** töltse ki a varázslót. Ez módosítja a DNS-beállításokat, majd lehetővé teszi a kijelölt szolgáltatások támogatásához szükséges egyéni DNS-rekordok hozzáadását.

Ha a névkiszolgálói rekordokat a Microsoftra módosította, és van webhelye, a névkiszolgálók visszaváltása helyett dns-rekordokat is felvehet a webhelyhez. További információt A DNS-rekordok frissítése úgy, hogy a webhely a jelenlegi [tárhelyszolgáltatónál maradjon](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)című cikk tartalmaz.


