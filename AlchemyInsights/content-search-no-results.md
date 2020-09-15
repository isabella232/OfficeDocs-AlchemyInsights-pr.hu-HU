---
title: Tartalmi találatok száma
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680649"
---
# <a name="no-results-from-content-searchexports"></a>A tartalom keresésének/exportálásának eredménye

A tartalmi kereséssel/exportálással kapcsolatos problémák oka az lehet, hogy bizonyos megfelelőségi biztonsági szűrőket egy bizonyos rendszergazdák állítanak be, és nem kommunikálnak a rendszergazdákkal.

A probléma megoldásához győződjön meg arról, hogy vannak-e olyan megfelelőségi biztonsági szűrők, amelyek az alábbi esetekben lehetnek így:
1. Csatlakozás a biztonsági és megfelelőségi központ Powershellhez
2. Futtassa az alábbi parancsmaggal található:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-szervezet $org