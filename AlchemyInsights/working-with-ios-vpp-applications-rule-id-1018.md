---
title: Az iOS VPP-alkalmazásokkal végzett műveletek szabály-azonosítója 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688948"
---
# <a name="working-with-ios-vpp-applications"></a>Az iOS VPP-alkalmazásokkal végezhető műveletek

A cikkből megtudhatja, [hogy miként kezelheti a mennyiségi vásárlással vásárolt iOS-alkalmazásokat a Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) segítségével, és megismerheti a Microsoft Intune szolgáltatásban elérhető Apple mennyiségi vásárlási program és a támogatás funkcióit.
  
 **Gyakori problémák:** "Egy iOS VPP alkalmazást Rendeltem a felhasználóknak, de a telepítés nem sikerült."
  
- Ez akkor fordulhat elő, ha egyetlen VPP-tokent használ több mobileszköz-kezelési szolgáltatónál. Az Apple-ből származó VPP-tokenek csak egy szolgáltatónál használhatók. Ha egy VPP-tokent több szolgáltatónál használt, újra fel kell töltenie a jogkivonatot a Intune-ra.

- A telepítés akkor is meghiúsulhat, ha a telepített példányok száma túllépi a licencek számát. A licencek használati jelentésének megtekintéséhez nyissa meg az **Intune Mobile apps** \> **app licencek** lapját. Ha meg szeretné tudni, hogy miként állíthatja vissza a licenceket a használatban, olvassa el [ezt a cikket.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
