---
title: A Yammer licencelési problémái
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148241"
---
# <a name="yammer-licensing-issues"></a>A Yammer licencelési problémái

A Yammer Nagyvállalati szolgáltatás használatához minden felhasználónak rendelkeznie kell licenccel, de a Yammer alapértelmezés szerint nem követeli meg, hogy a felhasználók nak legyen licencük a szolgáltatás eléréséhez. Ha egy rendszergazda módosítja a Yammer-licenccel nem rendelkező Microsoft 365-felhasználók blokkolásának beállítását, a Yammer Nagyvállalati licenccel nem rendelkező felhasználók nem férhetnek hozzá a Yammer-szolgáltatáshoz. További információ: [Yammer-felhasználói licencek kezelése az Office 365-ben](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Ha a licenceket eltávolítja a felhasználóktól, a Yammer csempe már nem jelenik meg, és más szolgáltatások a licenceltávolításával elrejthetik a szolgáltatásokat. Más esetekben a funkciók továbbra is megjelenhetnek, de a licenchozzárendelés működéséhez licenckiosztásszükséges.  

**A licenc nem frissül a felhasználó számára**  

Esetenként a felhasználóhoz licenc van rendelve, de továbbra sem tud hozzáférni a Yammerhez. A tömeges licenc-hozzárendelés ekor nagyobb a valószínűsége a késéseknek. Előfordulhat, hogy a Yammer-felhasználók nem ugyanabban a sorrendben frissülnek, mint az Azure AD-ben a licencek, mert a rendszer aszinkron módon fut. Várjon akár 24 órát, mielőtt megnyitna egy támogatási esetet a licencszinkronizálási problémák jelentéséhez.  

**Tömeges licenchozzárendelés**  

A licencek a felügyeleti központon vagy a PowerShell-parancsfájlokon keresztül rendelhetők hozzá. További információt a [Licencek hozzárendelése a felhasználókhoz](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) és [a Licencek hozzárendelése az Office 365 PowerShell használatával felhasználói fiókokhoz témakörben talál.](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell) 

A Microsoft támogatási szolgálata nem nyújt segítséget a parancsfájlok létrehozásához, de a Yammer licenc-hozzárendelésével kapcsolatos dokumentáció elérhető. További információt a [Yammer-licencek kezelése a Windows PowerShell használatával (Yammer-licencek kezelése) témakörben talál.](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell)