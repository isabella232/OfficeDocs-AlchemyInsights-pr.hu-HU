---
title: Read-Only a Maintenance (Karbantartás) üzenettel próbálkozik, amikor megkísérli használni SharePoint vagy OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: edcdea2f5c0647b92c230dd1d86549173e72997fc885195cde688b3b17710a2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53910548"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Read-Only a Maintenance (Karbantartás) üzenettel próbálkozik, amikor megkísérli használni SharePoint vagy OneDrive

Amikor megkísérli **használni** a karbantartáshoz szükséges SharePoint vagy OneDrive a következő esetek egyikére, a felhasználók csak olvasható üzenetet kaphatnak. 

-   Tervezett vagy aktív karbantartási tevékenység.  Ezeket az Üzenetközpontba [navigálva ellenőrizheti.](https://portal.office.com/adminportal/home#/messagecenter)
-   Magas prioritású aktív szolgáltatási incidens, amely előfordulhat. Az esetleges tanácsadókat és incidenseket a Szolgáltatás állapota csoportban [ellenőrizheti.](https://portal.office.com/adminportal/home#/servicehealth)
-   Kisebb automatikus helyreállítási forgatókönyv, amely a kiszolgálókon nem várt események miatt történhet, amelyek 30 percnél rövidebbek lehetnek. 
    
    Ezekhez a kisebb helyreállításhoz nem megjelenik az Üzenetközpont vagy a Szolgáltatás állapota bejegyzés, de hamarosan visszatér a normál állapothoz.

Nagyon néhány alkalommal azt figyeltünk meg, hogy a fent felsorolt három eset egyike okozhatja ezt, és a szolgáltatás vissza lett mondva, de a felhasználók böngészőjének gyorsítótára nem lett törölve.

Mielőtt a webhelyre navigál, próbálja meg kiürítni a böngésző gyorsítótárát.

1. A böngészőben Microsoft Edge **válassza** a Gépház , majd az Adatvédelem és biztonság **lehetőséget.**
2. A **Böngészés üríte alatt** válassza a Törölje a kívánt **adatokat lehetőséget.**
3. Válassza **a Cookie-k és mentett webhelyadatok**, majd a Törlése **lehetőséget.**

>[!Note] 
> Ezek a lépések eltérhetnek más böngészők, például a Mozilla Firefox vagy a Google Chrome használata esetén.

>[!Note] 
> Másik lehetőségként nyissa meg a SharePoint vagy OneDrive InPrivate-ablakban.