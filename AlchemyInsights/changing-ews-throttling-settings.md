---
title: Az EWS szabályozási beállításainak módosítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 4f0bea884153dc1ed8699ce12e0d017d18f5e57c
ms.sourcegitcommit: 53e5caab697ebfb434ccef3ef98b8f2bee579b41
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/02/2021
ms.locfileid: "50075899"
---
# <a name="changing-ews-throttling-settings"></a>Az EWS szabályozási beállításainak módosítása

Kérjük, futtassa automatizált tesztünket, amely lehetővé teszi az EWS-szabályozási házirend módosítását az áttelepítés ideje alatt. Vegye figyelembe, hogy az EWS-importok postaládánként 5 percenként 150 MB-ra korlátozva maradnak a futtatás után is; ha nagyobb átviteli sebességet szeretne elérni, kérjük, telepítsen át egyszerre több felhasználót.

Felhívjuk a figyelmét arra, hogy az EWS-szabályozási házirendek módosítása nincs hatással a következő áttelepítési típusokra (a Microsoft eszközeinek használatával): hibrid, átállásos/szakaszos (RPC/HTTP), IMAP, G Suite, nyilvános mappa vagy PST-importálási szolgáltatás.