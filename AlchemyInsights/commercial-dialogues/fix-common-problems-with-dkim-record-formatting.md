---
title: A DKIM rekordformázással kapcsolatos gyakori problémák megoldása
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: e55175e7613d220eaf956d3c7fd02213dcd5803d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323992"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>A DKIM rekordformázással kapcsolatos gyakori problémák megoldása

A DKIM beállításával kapcsolatos legtöbb probléma helytelen DNS-rekordokhoz kapcsolódik.

A DKIM beállítási problémáinak megoldásához ellenőrizze, hogy **a** DKIM CNAME rekord (nem TXT rekord) megfelelően van-e formázva. További információ: [A DKIM](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)manuális beállítása a Office 365.

Ha a DNS-rekordokkal kapcsolatos általános segítségre van szüksége, tekintse meg a [DNS-rekordok](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)létrehozása bármely DNS-szolgáltatónál a Office 365.

**Megjegyzés:** Miután tartománya DNS-szolgáltatónál létrehozott vagy frissült a DKIM DNS-rekordjai, meg kell várnia a DNS-rekordok propagálását.
