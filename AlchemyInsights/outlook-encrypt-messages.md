---
title: S/MIME a webes Outlookban
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
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772264"
---
# <a name="encrypt-email-messages-in-outlook"></a>E-mailek titkosítása az Outlookban

A Microsoft 365-üzenetek titkosítása a Microsoft Azure Rights Management (Azure RMS) verzióra épül, amely az Azure Information Protection része. Ha előfizetése tartalmazza az Azure Rights managementet vagy az Azure Information Protectiont, a Rights Management szolgáltatás **kézi engedélyezéséhez vagy aktiválásához nem kell semmilyen műveletet végrehajtania** .

Az ügyféltől érkező visszajelzések alapján a továbbiakban nem engedélyezzük az Exchange-levelezés szabályainak automatikus titkosítását, amely a bérlői fiókban lévő bizonyos típusú bizalmas információkat tartalmazó kimenő e-maileket automatikusan titkosítja. Ehelyett részletes útmutatást adunk arra vonatkozóan, hogy miként teheti ezt meg. Ha további információkra kíváncsi arról, hogy miként hozhat létre átviteli szabályt a bizalmas adatok titkosításához, olvassa el [ezt a cikket](https://aka.ms/OmeEtr).

- Ha a webes Outlookot használja (korábbi nevén **OWA**): e-mail írásakor egyszerűen kattintson a **védelem** az OWA alkalmazásban elemre. Ez a művelet a "nem továbbítható" engedélyt alkalmazza. Kattintson az **engedély módosítása** elemre, és válassza a **titkosítás** lehetőséget az üzenet titkosításához.

- Ha **Outlook-ügyfélprogramot**használ: Ha titkosított üzenetet szeretne küldeni az Outlook 2013 vagy 2016-ról, vagy a Mac Outlook 2016-ról, válassza a **Beállítások**  >  **engedélyei**lehetőséget, és válassza a szükséges védelem lehetőséget.

- Ha a címzetteknek vagy a külső partnereknek küldött **összes e-mailt automatikusan szeretné titkosítani** , létre kell hoznia egy e-mail-folyami átviteli szabályt az Exchange felügyeleti központban. [Ebben a támogatási cikkben](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)részletes útmutatást talál.

