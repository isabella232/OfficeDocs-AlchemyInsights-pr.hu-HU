---
title: A Sajátappok portál testreszabása
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7773"
- "9004350"
ms.openlocfilehash: e2d7cc165fce8be2e2c15d7d806917e309395d45
ms.sourcegitcommit: 688642f4ebc0f1c335e954e780bb9ec8893e2f3f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/20/2021
ms.locfileid: "49916783"
---
# <a name="customize-myapps-portal"></a>A Sajátappok portál testreszabása

1. A **Legutóbbi alkalmazások** lehetőség jelenleg csak a Sajátalkalmazások portál **Myapps Extention** gombja alatt érhető el.
2. Az Azure Active Directoryban (AD) létrehozott egyes gyűjtemények címét átnevezheti, a Minden alkalmazás címet **azonban nem.**
3. A Microsoft-alkalmazások nem távolíthatók el a MyApps gyűjteményből, és nem is részei egy másik gyűjteménykészletnek.
4. Az appindítót az Office portálon keresztül módosíthatja, a SajátAlkalmazások portálon keresztül azonban nem.
5. Az alkalmazások emblémájának testreszabásával kapcsolatos információkért lásd: Egyéni embléma [használata.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#use-a-custom-logo)
6. Egy alkalmazás URL-címének testreszabásához próbálkozzon az alábbi lépésekkel:
    - A **nagyvállalati** alkalmazások Gyűjtemények funkcióját használja. (Ezzel egy URL-címet kap, például: vagy a konfigurációja alapján https://myapps.microosft.com/customAppName.com hasonlót.)
    - Egy adott URL-címre mutató egyéni alkalmazást próbál ki a vállalati alkalmazásokban.
7. Az appok egyéni kezdőlap beállítása közzétett alkalmazásokhoz az [Azure AD alkalmazásproxyval](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-custom-home-page) történő beállításával kapcsolatban további információt arról, hogy miként konfigurálhatja a felhasználót egy egyéni kezdőlapra.
