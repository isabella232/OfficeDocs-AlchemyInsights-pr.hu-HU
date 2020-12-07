---
title: Microsoft Edge támogatása a Microsoft Defender alkalmazás-Gárda számára
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583582"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a>Microsoft Edge támogatása a Microsoft Defender alkalmazás-Gárda számára

A Windows 10 és a Microsoft Edge rendszerhez készült alkalmazás-őr hardveres elkülönítési megközelítést használ, amely lehetővé teszi, hogy egy felhasználó egy nem védett webhelyre navigáljon egy elszigetelt, hiper-V-os tárolótól, amely a fogadó operációs rendszertől elválasztva van.

A vállalati rendszergazdák a megbízható webhelyek, a felhőalapú erőforrások és a belső hálózatok listáját határozzák meg. Ha egy felhasználó olyan webhelyet látogat meg, amely nem szerepel a listán, a Microsoft Edge megnyitja a webhelyet a tárolóban. Ez azt jelenti, hogy ha a webhely kártékonynak tűnik, a gazdaszámítógép védett marad, és a támadó nem fog megjelenni a vállalati adatszolgáltatásban.

A bővítmények telepítése a tárolóban a Microsoft Edge 81-es verziójában érhető el, és egy házirenden keresztül is ellenőrizhető. Az ExtensionInstallForcelist-házirendben használt updateURL-címet semleges erőforrásként kell hozzáadni az alkalmazás-Gárda által használt hálózat-elkülönítési házirendekhez.

További információt a Microsoft [Edge támogatása a Microsoft Defender alkalmazás-Gárda számára](https://go.microsoft.com/fwlink/?linkid=2134229)című témakörben talál.
