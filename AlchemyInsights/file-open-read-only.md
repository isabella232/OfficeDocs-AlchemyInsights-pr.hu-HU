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
ms.openlocfilehash: e478572ea82e5ea11bac9fd7eacafb833253235d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813186"
---
# <a name="file-open-read-only"></a>Írás írásra megnyitott fájl

Előfordulhat, hogy a fájlok megnyitásakor a megnyitásuk csak olvashatóként történik. Bizonyos esetekben ez a nagyobb biztonság érdekében van így, például amikor az internetről nyit meg fájlokat, más esetekben pedig egy módosítható beállítás miatt. Íme néhány eset, amikor egy fájl csak olvashatóként nyílik meg, és néhány lépéssel módosíthatja azt.
  
 **A víruskereső miatt csak olvashatóan nyílik meg a fájl**
  
Egyes víruskereső programok írásra megnyitva védhetnek a potenciálisan nem biztonságos fájlok ellen. Előfordulhat, hogy a beállítások módosításához a víruskereső szolgáltatójától kell tájékozódni. A BitDefender például az alkalmazáskizárások hozzáadásáról a következő tartalommal rendelkezik: Alkalmazás- vagy folyamatkizárások hozzáadása a [Bitdefender vezérlőközpontjában.](https://aka.ms/AA6098i)
  
 **Írásra van-e állítva a fájltulajdonságok?**
  
A fájl tulajdonságainak ellenőrzéshez kattintson a jobb gombbal a fájlra, és válassza a Tulajdonságok parancsot. Ha be van jelölve a Csak olvasható attribútum, törölje a jelölését, és kattintson az OK gombra.
  
 **A tartalom védett nézetben van**
  
Az internetről és más, potenciálisan nem biztonságos helyekről származó fájlok a számítógépet kártékony vírusokat, férgeket vagy más típusú kártevőket tartalmazhatnak. Általában ez a helyzet az e-mail mellékletek és a letöltött fájlok esetében is. A számítógép védelme érdekében az ilyen, potenciálisan nem biztonságos helyekről származó fájlok védett nézetben nyithatók meg. A védett nézet használatával úgy olvashatja el a fájlokat és megtekintheti a tartalmát, hogy közben csökkenti a kockázatokat. A védett nézetről és a beállítások módosításáról a következő cikkben olvashat bővebben: Mi [a védett nézet?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)
  
 **Megtelt a OneDrive?**
  
Ha a fájlt a OneDrive-on tárolja, és megtelt a OneDrive-tárterülete, akkor mindaddig nem fogja tudni menteni a dokumentumot, amíg a kiosztott tárterület alá nem áll. A OneDrive-on a szabad terület ellenőrzéséhez kattintson a OneDrive ikonra az értesítési központban, és válassza a Tárterület kezelése gombra kattintva, vagy a ikonra kattintva jelentkezzen be, és jegyezze fel a felhasznált terület mennyiségét a képernyő bal alsó [https://onedrive.live.com](https://onedrive.live.com) részén.
  
 **Aktiválva van az Office?**
  
Ha az Office nincs aktiválva, vagy ha lejárt az előfizetése, akkor lehet, hogy csak olvasható csökkentett szolgáltatáskészletű üzemmódban van. Az Office aktiválásának mikéntjére vonatkozó információkért lásd: "Nem licencelt termék" aktiválási hibaüzenetek az [Office-ban.](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
  
 **Ha minden más kudarcotik...**
  
- Próbálkozzon a számítógép újraindításával
    
- Office-frissítések telepítése
    
- Az Office online javítása
    

