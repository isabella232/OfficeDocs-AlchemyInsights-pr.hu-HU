---
title: Az iOS VPP-alkalmazások 1018-as szabályának alkalmazása
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719959"
---
# <a name="working-with-ios-vpp-applications"></a>Az iOS VPP-alkalmazások kal való együttműködés

Olvassa [el A Microsoft Intune-nal egy mennyiségi vásárlási program keretében vásárolt iOS-alkalmazások kezelése](https://docs.microsoft.com/intune/vpp-apps-ios) című, a Microsoft Intune-ban található funkciók, korlátozások és az Apple mennyiségi vásárlási programjának használatának lépéseit és a Microsoft Intune-ban nyújtott támogatás használatát.
  
 **Gyakori problémák:** "IOS VPP alkalmazást rendeltem a felhasználókhoz, de a telepítés nem sikerült."
  
- Ez akkor fordulhat elő, ha egyetlen VPP-jogkivonatot használ több mobileszköz-felügyeleti szolgáltató között. Az Apple VPP-tokenjeit csak egy szolgáltatónál lehet használni. Ha több szolgáltatóval használt VPP-jogkivonatot, újra fel kell töltenie a jogkivonatot az Intune-ba.

- A telepítés akkor is sikertelen lehet, ha a telepítések száma meghaladja a licencek számát. A licencek használati jelentésének megtekintéséhez nyissa meg az **Intune Mobile apps** \> **alkalmazáslicencek lapját.** A használatban lévő licencek visszaigénylésének módjáról [ebben a cikkben olvashat.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
