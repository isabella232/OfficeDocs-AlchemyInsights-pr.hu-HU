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
ms.openlocfilehash: 9e258cfc70c57fe787830d659dc52f4696768bea164d3be9ce7bcb9e7123c5a9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971017"
---
# <a name="verify-your-domain"></a>Verify your domain

 **A rekord valószínűleg nem frissült az interneten keresztül.**
  
Az új rekordot általában csak néhány percig tart, de időnként akár néhány óráig is eltarthat. 
  
- Ha ilyen sokáig várt, ellenőrizze, hogy pontosan a PONTOS értéket másolta-e be a DNS-szolgáltatóNÁL található TXT rekordba. Gyakori probléma, hogy a rekord nem tartalmazza az "MS=" részt. Arra is szükség van!

- Egyes DNS-szolgáltatónál további lépéssel mentenie kell a zónafájlt (ahol a DNS-rekordot tárolja), hogy az szerte az interneten frissülni fog. Győződjön meg arról, hogy mentette a módosításokat, hogy a Microsoft lássa és ellenőrizni tudja a rekordot.
