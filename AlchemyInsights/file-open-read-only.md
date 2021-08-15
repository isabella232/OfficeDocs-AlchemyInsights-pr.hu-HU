---
title: Írás írásra megnyitott fájl
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: fb75f7ac5b8c7023f0258a567becdc5d023476b5e905d8f2cc17479faea76af1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54029806"
---
# <a name="file-open-read-only"></a>Írás írásra megnyitott fájl

Előfordulhat, hogy a fájlok megnyitásakor a megnyitásuk csak olvashatóként történik. Bizonyos esetekben ez a nagyobb biztonság érdekében van így, például amikor az internetről nyit meg fájlokat, más esetekben pedig egy módosítható beállítás miatt. Íme néhány eset, amikor egy fájl csak olvashatóként nyílik meg, és néhány lépéssel módosíthatja azt.
  
 **A víruskereső miatt csak olvashatóan nyílik meg a fájl**
  
Egyes víruskereső programok írásra megnyitva védhetnek a potenciálisan nem biztonságos fájlok ellen. Előfordulhat, hogy a beállítások módosításához a víruskereső szolgáltatójától kell tájékozódni. A BitDefender például az alkalmazáskizárások hozzáadásáról a következő tartalommal rendelkezik: Alkalmazás- vagy folyamatkizárások hozzáadása a [Bitdefender vezérlőközpontjában.](https://aka.ms/AA6098i)
  
 **Írásra van-e állítva a fájltulajdonságok?**
  
A fájl tulajdonságainak ellenőrzéshez kattintson a jobb gombbal a fájlra, és válassza a Tulajdonságok parancsot. Ha be van jelölve a Csak olvasható attribútum, törölje a jelölését, és kattintson az OK gombra.
  
 **A tartalom védett nézetben van**
  
Az internetről és más, potenciálisan nem biztonságos helyekről származó fájlok a számítógépet kártékony vírusokat, férgeket vagy más típusú kártevőket tartalmazhatnak. Általában ez a helyzet az e-mail mellékletek és a letöltött fájlok esetében is. A számítógép védelme érdekében az ilyen, potenciálisan nem biztonságos helyekről származó fájlok védett nézetben nyithatók meg. A védett nézet használatával úgy olvashatja el a fájlokat és megtekintheti a tartalmát, hogy közben csökkenti a kockázatokat. A védett nézetről és a beállítások módosításáról a következő cikkben olvashat bővebben: Mi [a védett nézet?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)
  
 **Megtelt OneDrive?**
  
Ha a fájlt a OneDrive tárolja, OneDrive tárterülete megtelt, nem fogja tudni menteni a dokumentumot, amíg a kiosztott tárterület alá nem áll. Az OneDrive-ban a szabad terület ellenőrzéséhez kattintson az OneDrive ikonra az értesítési központban, és válassza a Tárhely kezelése gombra kattintva, vagy a ikonra kattintva jelentkezzen be, és jegyezze fel a felhasznált terület mennyiségét a képernyő bal alsó [https://onedrive.live.com](https://onedrive.live.com) részén.
  
 **Aktiválva Office?**
  
Ha Office nincs aktiválva, vagy ha előfizetése lejárt, akkor lehet, hogy csak olvasható csökkentett szolgáltatáskészletű üzemmódban van. Az aktiválási hibák aktiválásának mikéntjére vonatkozó Office: "Nem licencelt termék" aktiválási hibaüzenetek a [Office.](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
  
 **Ha minden más kudarcotik...**
  
- Próbálkozzon a számítógép újraindításával
    
- Office frissítések telepítése
    
- Online javítás Office
    

