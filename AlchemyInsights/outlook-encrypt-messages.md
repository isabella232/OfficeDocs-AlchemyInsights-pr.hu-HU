---
title: S/MIME a Webes Outlookban
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 7184ffd68f56639a8bcb87e9c6cab88388868103
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764874"
---
# <a name="encrypt-email-messages-in-outlook"></a>E-mailek titkosítása az Outlookban

A Microsoft 365 üzenettitkosítás a Microsoft Azure Tartalomvédelmi Szolgáltatás (Azure RMS) szolgáltatásra épül, amely az Azure Information Protection része. Ha előfizetése tartalmazza az Azure Rights Management vagy az Azure Information Protection szolgáltatást, nem kell semmilyen műveletet tennie a tartalomvédelmi szolgáltatás **manuális engedélyezéséhez vagy aktiválásához.**

Az ügyfelek visszajelzései alapján a továbbiakban nem engedélyezzük az Exchange levelezési szabályainak automatikus anno a bérlőben bizonyos típusú bizalmas adatokat tartalmazó kimenő e-mailek titkosítását. Ehelyett részletes utasításokat adunk arra vonatkozóan, hogy ezt hogyan teheti meg. A bizalmas adatok titkosítására szolgáló átviteli szabályok létrehozásáról a [cikkben](https://aka.ms/OmeEtr)olvashat további részletekről.

- Ha a Webes Outlookot (korábbi ideig **OWA)** használja: E-mail írásakor egyszerűen kattintson a **Védelem** az OWA-ban gombra. Ez a "Ne továbbítsa" engedélyt alkalmazza. Kattintson **a Módosítás gombra,** és válassza a **Titkosítás** lehetőséget az üzenet titkosításához.

- **Outlook-ügyfél**használata esetén : Titkosított üzenet küldéséhez az Outlook 2013-ból vagy 2016-ból, illetve a Mac Outlook 2016-ból, válassza a **Beállítások** > **engedélyek**lehetőséget, majd válassza ki a szükséges védelmi beállítást.

- Az egyes címzetteknek vagy külső partnerszervezeteknek küldött **összes e-mail automatikus titkosításához** létre kell hoznia egy levelezési átviteli szabályt az Exchange Felügyeleti központban. Részletes utasításokat ebben a [támogatási cikkben](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities)talál.

