---
title: Az EWS szabályozási beállításainak módosítása
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
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: f99bb449b542760c6c8d51ee399c774fbe36e3f7f40520b5eb23f39d9d7c08dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53968379"
---
# <a name="changing-ews-throttling-settings"></a>Az EWS szabályozási beállításainak módosítása

Kérjük, futtassa automatizált tesztünket, amely lehetővé teszi az EWS-szabályozási házirend módosítását az áttelepítés ideje alatt. Vegye figyelembe, hogy az EWS-importok postaládánként 5 percenként 150 MB-ra korlátozva maradnak a futtatás után is; ha nagyobb átviteli sebességet szeretne elérni, kérjük, telepítsen át egyszerre több felhasználót.

Felhívjuk a figyelmét arra, hogy az EWS-szabályozási házirendek módosítása nincs hatással a következő áttelepítési típusokra (a Microsoft eszközeinek használatával): hibrid, átállásos/szakaszos (RPC/HTTP), IMAP, G Suite, nyilvános mappa vagy PST-importálási szolgáltatás.