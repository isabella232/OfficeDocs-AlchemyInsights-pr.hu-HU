---
title: Yammer licencelési problémák
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 3ec764ece9cb7be933e9e2cd002379898522790528b0fa586ab501424b00cd7b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989731"
---
# <a name="yammer-licensing-issues"></a>Yammer licencelési problémák

Az Yammer Nagyvállalati verzió szolgáltatáshoz minden felhasználónak licenccel kell Yammer, de alapértelmezés szerint nincs szükség licencre a felhasználóknak a szolgáltatás eléréséhez. Ha egy rendszergazda úgy módosítja a beállítást, hogy Microsoft 365 licenccel nem rendelkező Yammer, a Yammer Nagyvállalati verzió-licenccel nem rendelkező felhasználók nem férhetnek hozzá a Yammer szolgáltatáshoz. További információt a Felhasználói [licencek Yammer kezelése a](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) Office 365 

Amikor licenceket távolít el a felhasználóktól, a Yammer csempe nem jelenik meg, és más szolgáltatások a licencek eltávolításával elrejtik a funkciókat. Más esetekben a funkciók továbbra is megjelenhetnek, de működéséhez licenc-hozzárendelésre van szükség.  

**Nem frissül a felhasználó licence**  

Időnként előfordulhat, hogy egy felhasználóhoz licenc van rendelve, de továbbra sem fér hozzá a Yammer. A késések nagyobb valószínűséggel fordulnak elő, ha tömeges licenc-hozzárendelés van folyamatban. Yammer, hogy a felhasználók frissítése nem ugyanabban a sorrendben történt, mint ahogyan a licencek módosulnak az Azure AD-ban, mert a rendszer aszinkron módon fut. Várjon akár 24 órát, mielőtt megnyit egy támogatási esetet, és jelentse a licencszinkronizálási problémákat.  

**Tömeges licenc-hozzárendelés**  

A licenceket a felügyeleti központon vagy a PowerShell-parancsprogramon keresztül lehet hozzárendelni. További információ: [Licencek](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) hozzárendelése felhasználókhoz és Licencek hozzárendelése felhasználói fiókokhoz [a Office 365 PowerShell használatával.](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell) 

A Microsoft ügyfélszolgálata nem nyújt segítséget parancsfájlok létrehozásához, de a Yammer hozzárendelés dokumentációja áll rendelkezésre. További információt a [Licenclicencek kezelése Yammer a](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell)következő Windows PowerShell.