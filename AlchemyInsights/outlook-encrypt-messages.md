---
title: S/MIME a Webes Outlook
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: bef87baafdbaf9346f99f1ff54aaa83bc9173c70f1412ea00afb717c15a8014c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54010726"
---
# <a name="encrypt-email-messages-in-outlook"></a>E-mailek titkosítása a Outlook

Microsoft 365 Az Üzenettitkosítás az Azure Microsoft Azure Rights Management (Azure RMS) szolgáltatásra épül, amely az Azure Information Protection része. Ha előfizetése tartalmaz Azure Tartalomvédelmi szolgáltatások Azure Information Protection **szolgáltatást,** akkor semmit sem kell tennie a Rights Management Szolgáltatás manuális engedélyezéséhez vagy aktiválásához.

Az ügyfelek visszajelzései alapján a továbbiakban nem engedélyezünk e-mail-forgalomra vonatkozó szabályokat Exchange bérlője bizonyos típusú bizalmas adatait tartalmazó kimenő e-mailek automatikus titkosítására. Ehelyett részletes útmutatást nyújtunk arról, hogy miként használhatja ezt a szolgáltatást. A bizalmas adatok titkosítására vonatkozó átviteli szabály létrehozásáról további információt ebben a [cikkben talál.](https://aka.ms/OmeEtr)

- Ha webes Outlook (korábbi nevén **OWA):** Üzenet írása esetén egyszerűen  kattintson a Védelem az Outlook Web Appban gombra. Ez a "Nem továbbítja" engedélyt fogja alkalmazni. Kattintson **az Engedély módosítása elemre,** és válassza a Titkosítás **lehetőséget,** ha csak az üzenetet titkosítja.

- Ha **Outlook ügyfélprogramot** használ: Ha titkosított üzenetet Outlook 2013-as vagy 2016-os vagy Mac Outlook 2016-es vagy Mac Outlook 2016, válassza a Beállítások engedélyek lehetőséget, majd válassza ki a kívánt védelmi  >  beállítást.

- A **bizonyos címzetteknek** vagy külső partnerszervezeteknek küldött összes e-mail automatikus titkosításához létre kell hoznia egy e-mail-forgalom átviteli szabályát a Exchange felügyeleti központban. Részletes útmutatást ebben a támogatási [cikkben talál.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)

