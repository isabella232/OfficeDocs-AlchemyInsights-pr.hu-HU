---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 4a34de7fa2aaaae365cf4562d31590d4b5fb7544
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51770993"
---
# <a name="verify-your-domain"></a>Verify your domain

 **A rekord valószínűleg nem frissült az interneten keresztül.**
  
Az új rekordot általában csak néhány percig tart, de időnként akár néhány óráig is eltarthat. 
  
- Ha ilyen sokáig várt, ellenőrizze, hogy pontosan a PONTOS értéket másolta-e be a DNS-szolgáltatóNÁL található TXT rekordba. Gyakori probléma, hogy a rekord nem tartalmazza az "MS=" részt. Arra is szükség van!

- Egyes DNS-szolgáltatónál további lépéssel mentenie kell a zónafájlt (ahol a DNS-rekordot tárolja), hogy az szerte az interneten frissülni fog. Győződjön meg arról, hogy mentette a módosításokat, hogy a Microsoft lássa és ellenőrizni tudja a rekordot.
