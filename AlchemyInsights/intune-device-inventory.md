---
title: Intune-eszköz készlete
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667880"
---
# <a name="intune-device-inventory"></a>Intune-eszköz készlete

Az eszközök Blade segítségével a rendszergazda betekintést adhat az Intune-eszközökhöz eszközönként. A megjelenített adatok a következők: hardver, az észlelt alkalmazások, az eszköz megfelelőségi állapota és az eszköz konfigurációja állapota.

A hardverek és a felfedezett alkalmazások leltározása hét napos ciklusban történik. Az alkalmazások és a hardver bizonyos elemei eltérőek lehetnek az eszköz operációs rendszertől függően, és hogy az eszköz személyes vagy vállalati tulajdonú-e.

További információt az [eszközök adatainak megtekintése az Intune-ban](https://docs.microsoft.com/intune/device-inventory)című témakörben találhat.

**GYIK**

K: nem kapok teljes leltározási listát az Intune által regisztrált Windows-eszközökön lévő alkalmazásokról. miért ne?

A: jelenleg csak a modern alkalmazások jelennek meg a Windows 10 rendszerű PC-ken, amelyeket vállalati eszközökként azonosítottak. Az Intune nem gyűjt információkat az ilyen eszközökön telepített Win32-alkalmazásokról.

K.: Miért nem minden eszközről gyűjtenek telefonszámot?

A: az Intune-ban a vállalati eszközökként kategorizált telefonok esetében a rendszer nem azonosítja a teljes telefonszámot, ha például mobileszköz-készletezési jelentést futtat. A bringa-you-Own-Phone-telefonszámokat mindig részlegesen maszkolt csillagokkal (* * * *), és csak az utolsó négy számjegyet jeleníti meg.