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
ms.openlocfilehash: 16916d5f16f763d87ce0d5ef830e741279c9f4df
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818038"
---
# <a name="changing-ews-throttling-settings"></a>Az EWS szabályozási beállításainak módosítása

Kérjük, futtassa automatizált tesztünket, amely lehetővé teszi az EWS-szabályozási házirend módosítását az áttelepítés ideje alatt. Vegye figyelembe, hogy az EWS-importok postaládánként 5 percenként 150 MB-ra korlátozva maradnak a futtatás után is; ha nagyobb átviteli sebességet szeretne elérni, kérjük, telepítsen át egyszerre több felhasználót.

Felhívjuk a figyelmét arra, hogy az EWS-szabályozási házirendek módosítása nincs hatással a következő áttelepítési típusokra (a Microsoft eszközeinek használatával): hibrid, átállásos/szakaszos (RPC/HTTP), IMAP, G Suite, nyilvános mappa vagy PST-importálási szolgáltatás.