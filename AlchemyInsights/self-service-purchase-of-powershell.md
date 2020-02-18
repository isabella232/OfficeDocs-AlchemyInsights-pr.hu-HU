---
title: A PowerShell önkiszolgáló vásárlása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3516"
ms.openlocfilehash: 5e47e08e3309b3d58908e10ee06021da00f230bb
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091713"
---
# <a name="self-service-purchase-of-powershell"></a>A PowerShell önkiszolgáló vásárlása

Az MSCommerce PowerShell modul használatához telepítenie kell azt egy TLS 1.2-es (helyi rendszergazdai engedélyekkel rendelkező) Windows 10-es eszközre.  Importálja és csatlakozzon az MSCommerce modulhoz.  Amikor a rendszer kéri a bejelentkezést, globális vagy számlázási rendszergazdai szerepkör hitelesítő adatait kell használnia.  

Ha nem rendelkezik TLS 1.2-vel, a következő hibaüzenet jelenhet meg a házirend betöltésekor vagy frissítésekor:

*ErrorMessage -Az alapul szolgáló kapcsolat megszakadt: Váratlan hiba történt a küldéssorán.*



