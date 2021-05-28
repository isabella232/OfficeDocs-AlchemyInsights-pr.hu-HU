---
title: Két hanghívás felvétele két hangra
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: 18c68fee514681b2a81c3cfa022c29ce83834f22
ms.sourcegitcommit: 610a5d950cdf488870601762ef52d881e3e22a48
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696960"
---
# <a name="11-call-recording"></a>Két hanghívás felvétele két hangra

Ha a **Rögzítés elindítani** gomb szürkén jelenik meg egy az egyhez hívásban, módosítania kell az érintett felhasználó házirendbeállítását.   

2021. május 31-től bevezetünk egy új hívási házirendet az *AllowCloudRecordingForCalls* Teams hívási házirendben. A változás előtt az kéthívásos felvétel vezérlése az *AllowCloudRecording* Teams szabály szerint történik. Ez a változás az Üzenetközpont bejegyzésében [található: (Frissítve) 1:1 Hívásrögzítési házirend – bevezetés.](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)  

*AllowCloudRecordingForCalls*   hívási házirend beállítás alapértelmezés **szerint $False** van beállítva. Ha azt szeretné, hogy az összes felhasználó ne rögzítsen két hanghívást, akkor nincs semmilyen teendőja.  

Ha engedélyezni szeretné a hívásrögzítést az összes felhasználó számára két Teams a PowerShellben, futtassa az alábbi parancsmagot: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Másik lehetőségként létrehozhat egy új házirendet, és beállíthatja az  **-AllowCloudRecordingForCalls** $true és hozzárendelheti a házirendet a felhasználókhoz. 

További információ: Hívásrögzítési házirend-vezérlők [(majdnem!) Itt .](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668)
