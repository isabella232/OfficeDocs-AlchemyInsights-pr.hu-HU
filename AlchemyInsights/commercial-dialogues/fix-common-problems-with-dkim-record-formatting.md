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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746834"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>A DKIM rekordformázással kapcsolatos gyakori problémák megoldása

A DKIM beállításával kapcsolatos legtöbb probléma helytelen DNS-rekordokhoz kapcsolódik.

A DKIM beállítási problémáinak megoldásához ellenőrizze, hogy **a** DKIM CNAME rekord (nem TXT rekord) megfelelően van-e formázva. További információ: A DKIM kézi beállítása az [Office 365-ben.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)

Ha a DNS-rekordokkal kapcsolatos általános segítségre van szüksége, tekintse át A DNS-rekordok létrehozása bármely DNS-szolgáltatónál az [Office 365 szolgáltatáshoz című cikkeket.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

> [!NOTE]
> Miután a tartomány DNS-szolgáltatónál létrehozott vagy frissült a DKIM DNS-rekordok, meg kell várnia a DNS-rekordok propagálását.
