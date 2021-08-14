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
ms.openlocfilehash: 5b3dc2338843906fbc7151322b82f304b4ed04b28d8ceb349f2705c309cdeae8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930063"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>A DKIM rekordformázással kapcsolatos gyakori problémák megoldása

A DKIM beállításával kapcsolatos legtöbb probléma helytelen DNS-rekordokhoz kapcsolódik.

A DKIM beállítási problémáinak megoldásához ellenőrizze, hogy **a** DKIM CNAME rekord (nem TXT rekord) megfelelően van-e formázva. További információ: A [DKIM](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)manuális beállítása a Office 365.

Ha a DNS-rekordokkal kapcsolatos általános segítségre van szüksége, tekintse át a [DNS-rekordok](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)létrehozása bármely DNS-szolgáltatónál a Office 365.

> [!NOTE]
> Miután a tartomány DNS-szolgáltatónál létrehozott vagy frissült a DKIM DNS-rekordok, meg kell várnia a DNS-rekordok propagálását.
