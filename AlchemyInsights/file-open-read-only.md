---
title: Fájl megnyitása írásvédett
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 2fdb4f048c2bee022a49c2cca2ce9770f42a87a2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745587"
---
# <a name="file-open-read-only"></a>Fájl megnyitása írásvédett

Előfordulhat, hogy a fájlok megnyitásakor csak olvashatóként nyílik meg. Bizonyos esetekben ez a biztonság, például a fájlok internetről való megnyitásakor, illetve máskor is előfordulhat, hogy ez a beállítás a módosítható beállításnak köszönhető. Íme néhány példa arra, hogy egy fájl írásvédett módban nyílik meg, és néhány lépésben megteheti a módosítást.
  
 **A víruskeresők azt okozzák, hogy csak írásvédett módban nyílnak meg**
  
Egyes víruskereső programok csak olvashatóan tudják megvédeni a fájlokat a potenciálisan nem biztonságos fájlokból. Ha meg szeretné tudni, hogy miként igazíthatja ezeket a beállításokat, előfordulhat, hogy meg kell vizsgálnia a víruskereső szolgáltatóját. BitDefender (például) tartalma az alkalmazások kivételének hozzáadásához: [Hogyan vehet fel alkalmazást vagy folyamat kizárását a BitDefender Control Center alkalmazásban](https://aka.ms/AA6098i).
  
 **A fájl tulajdonságai csak olvashatók legyenek?**
  
A fájl tulajdonságainak ellenőrzéséhez kattintson a jobb gombbal a fájlra, és válassza a Tulajdonságok parancsot. Ha a írásvédett attribútum be van jelölve, akkor törölje a jelet, és kattintson az OK gombra.
  
 **A tartalom védett nézetben van**
  
Az internetről és más, esetleg nem biztonságos helyekről származó fájlok tartalmazhatnak vírusokat, férgeket vagy más típusú kártevőket, amelyek károsíthatják a számítógépre. Ez a helyzet általában az e-mail-mellékletek vagy a letöltött fájlok esetén is. A számítógép védelme érdekében a nem biztonságos helyekről származó fájlok védett nézetben nyílnak meg. A védett nézet használatával elolvashatja a fájlt, és megtekintheti a tartalmát, miközben csökkenti a kockázatokat. A védett nézetről és a beállítások módosításáról a [védett nézet](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653) című témakörben olvashat bővebben.
  
 **Teljes a OneDrive?**
  
Ha a fájl a OneDrive van tárolva, és a OneDrive tárterülete megtelik, akkor a program nem menti a dokumentumot, amíg el nem éri a kiosztott tárterületét. Az OneDrive-on lévő szabad terület ellenőrzéséhez kattintson a OneDrive ikonra az értesítési központban, és válassza a tárterület kezelése lehetőséget, vagy lépjen a [https://onedrive.live.com](https://onedrive.live.com) képernyő bal alsó részén lévő szabad területhez.
  
 **Aktivált az Office?**
  
Ha az Office nincs aktiválva, vagy lejárt az előfizetése, akkor csak olvasható csökkentett módban lehet. Az Office aktiválásához további információt a következő témakörben talál: nem [licencelt termék-és aktiválási hibák az Office-ban](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).
  
 **Ha minden kötél szakadt meg...**
  
- Próbálkozzon a számítógép újraindításával
    
- Office-frissítések telepítése
    
- Az Office Online javításának elvégzése
    

