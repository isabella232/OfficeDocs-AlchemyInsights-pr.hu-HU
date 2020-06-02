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
ms.openlocfilehash: 6bbbf8722dacb8b7d5191d57ce1055a48dcb4dd0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511510"
---
# <a name="encrypt-email-messages-in-outlook"></a>E-mailek titkosítása az Outlookban

A Microsoft 365 üzenettitkosítás a Microsoft Azure Tartalomvédelmi Szolgáltatás (Azure RMS) szolgáltatásra épül, amely az Azure Information Protection része. Ha előfizetése tartalmazza az Azure Rights Management vagy az Azure Information Protection szolgáltatást, nem kell semmilyen műveletet tennie a tartalomvédelmi szolgáltatás **manuális engedélyezéséhez vagy aktiválásához.**

Az ügyfelek visszajelzései alapján a továbbiakban nem engedélyezzük az Exchange levelezési szabályainak automatikus anno a bérlőben bizonyos típusú bizalmas adatokat tartalmazó kimenő e-mailek titkosítását. Ehelyett részletes utasításokat adunk arra vonatkozóan, hogy ezt hogyan teheti meg. A bizalmas adatok titkosítására szolgáló átviteli szabályok létrehozásáról a [cikkben](https://aka.ms/OmeEtr)olvashat további részletekről.

- Ha a Webes Outlookot (korábbi ideig **OWA)** használja: E-mail írásakor egyszerűen kattintson a **Védelem** az OWA-ban gombra. Ez a "Ne továbbítsa" engedélyt alkalmazza. Kattintson **a Módosítás gombra,** és válassza a **Titkosítás** lehetőséget az üzenet titkosításához.

- **Outlook-ügyfél**használata esetén : Titkosított üzenet küldéséhez az Outlook 2013-ból vagy 2016-ból, illetve a Mac Outlook 2016-ból, válassza a **Beállítások**  >  **engedélyek**lehetőséget, majd válassza ki a szükséges védelmi beállítást.

- Az egyes címzetteknek vagy külső partnerszervezeteknek küldött **összes e-mail automatikus titkosításához** létre kell hoznia egy levelezési átviteli szabályt az Exchange Felügyeleti központban. Részletes utasításokat ebben a [támogatási cikkben](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)talál.

