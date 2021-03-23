---
title: Importálás és exportálás a Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036124"
---
# <a name="import-and-export-from-yammer"></a>Importálás és exportálás a Yammer

**Importálás**

A felhasználói importálási beállítások attól függően változnak, hogy Yammer a [Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)natív módjában van-e, vagy sem.

- **Nem natív** mód: A felhasználók importálhatók csoportokba a Hozzáadás címjegyzékből [(legfeljebb](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) 100 felhasználóval) használatával a csoportbeállítások között, illetve a hálózatba a hálózati rendszergazda tömeges frissítésével. [](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users)
- **Natív mód:** A csoporttagságot és a hálózati tagsági műveleteket a [Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users)Felügyeleti portálon, az [Azure AD portálon](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)vagy egy másik Azure AD-beállítással kell végrehajtani. A natív módban található hálózatok többé nem férnek hozzá a tömeges frissítéshez és más korábbi funkciókhoz.

> [!IMPORTANT]
> Yammer még akkor sem támogatja a tartalom importálását a hálózati rendszergazdából, ha az adatexportozási funkciót egy másik hálózaton használták. A tartalmakat újra közzétenheti partnermegoldások vagy az Yammer REST API-k.

**Exportálás**

[A hálózati adatok hálózati rendszergazdai](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) exportálása lehetővé teszi a tartalom exportálását Yammer hálózatokból, beleértve az üzeneteket és fájlokat is. A mellékletek rendkívül nagy méretűek, és az exportálások befejeződését is jelentősen igénybe veszi. Azt javasoljuk, hogy az aktív hálózatok exportálása az adatexportálti [API](https://developer.yammer.com/docs/data-export-api) használatával napi vagy heti adattömbökbe. Erre a célra a Microsoft ügyfélszolgálata nem biztosít egyéni parancsfájlokat.

Külön [GDPR-exportálás létezik](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) a tartalmak egy adott felhasználónak való exportálására.