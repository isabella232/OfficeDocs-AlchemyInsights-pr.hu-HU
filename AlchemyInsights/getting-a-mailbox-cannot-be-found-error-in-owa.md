---
title: az OWA alkalmazásban nem található az 126-ös postaláda-hiba
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 9a8897767ebfebac5807116251634c615ef6767d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47706752"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Nem található a postaláda hibája a webes Outlookban?

Ha a webes Outlookot használja, és a **postaládáját nem sikerült megtalálni** , akkor a webes Outlookhoz való csatlakozáshoz használt fiók nem rendelkezik Exchange Online-licenccel, ezért a fiókhoz nincs társítva postaláda. A rendszergazda az alábbi lépésekkel rendelhet licencet a fiókjához:

1. Nyissa meg a [Microsoft 365 felügyeleti központját](https://portal.office.com/adminportal/home#/homepage) , és nyissa meg az **aktív felhasználók** szakaszt a **felhasználók** csoportban, és jelölje ki azt a felhasználót, aki látta a hibát.

2. A megnyíló felhasználói lapon nyissa meg a **licencek és alkalmazások** szakaszt, válassza ki a megfelelő **tartózkodási helyet** , és rendelje hozzá az Exchange Online-t tartalmazó licencet (bontsa ki a licencet a részletek megjelenítéséhez). Ha végzett, kattintson a **módosítások mentése**gombra.
