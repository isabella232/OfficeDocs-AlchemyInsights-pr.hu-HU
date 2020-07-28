---
title: Intune-eszközleltár
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439655"
---
# <a name="intune-device-inventory"></a>Intune-eszközleltár

Az Eszközök panel eszközalapon betekintést nyújt a rendszergazdai eszközökbe az Intune-ban. A megjelenített információk a következők: hardver, felderített alkalmazások, eszközmegfelelőségi állapot és eszközkonfigurációállapota.

A hardverek és a felderített alkalmazások készletadatait hétnapos ciklusban gyűjtik. A jelentett alkalmazások és hardverelemek az eszköz operációs rendszerétől és attól függően változnak, hogy az eszköz személyes vagy vállalati tulajdonban van-e.

További információ: [Az eszköz részletei az Intune-ban.](https://docs.microsoft.com/intune/device-inventory)

**GYIK**

K: Nem kapom meg az Intune által regisztrált Windows-eszközökön található alkalmazások teljes leltárlistáját. miért ne?

A: Jelenleg csak a vállalati eszközként azonosított Windows 10-es számítógépeken csak a modern alkalmazások jelennek meg. Az Intune nem gyűjt adatokat az ezekre az eszközökre telepített Win32-alkalmazásokról.

K: Miért nem gyűjtik a telefonszámokat az összes eszközről?

A: Az Intune-ban vállalati eszközként kategorizált telefonok nem azonosulnak a teljes telefonszámukkal, ha például mobileszköz-leltárjelentést futtat. Bring-you-device telefonszámok mindig részben maszkolt csillaggal (****), és csak az utolsó négy számjegy.