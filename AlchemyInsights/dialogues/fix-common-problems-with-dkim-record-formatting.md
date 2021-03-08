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
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524395"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>A DKIM rekordformázással kapcsolatos gyakori problémák megoldása

A DKIM beállításával kapcsolatos legtöbb probléma helytelen DNS-rekordokhoz kapcsolódik.

A DKIM beállítási problémáinak megoldásához ellenőrizze, hogy **a** DKIM CNAME rekord (nem TXT rekord) megfelelően van-e formázva. További információt a DKIM manuális beállítását az [Office 365-ben az Office 365-ben](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).

Ha általános segítségre van szüksége a DNS-rekordokhoz, tekintse át a DNS-rekordok létrehozása bármely DNS-szolgáltatónál az [Office 365-nek című cikkt.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

> [!NOTE]
> Miután a tartomány DNS-szolgáltatónál létrehozott vagy frissít egy DKIM DNS-rekordot, meg kell várnia a DNS-rekordok propagálását.
