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
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657278"
---
# <a name="yammer-licensing-issues"></a>Yammer licencelési problémák

Minden felhasználónak rendelkeznie kell licenccel a Yammer nagyvállalati szolgáltatás használatához, de alapértelmezés szerint a Yammer nincs szükség ahhoz, hogy a felhasználók hozzáférjenek a szolgáltatáshoz. Ha a rendszergazda módosítja a beállítást a Microsoft 365-felhasználók Yammer-licencek nélküli blokkolására, a Yammer nagyvállalati licenccel nem rendelkező felhasználók nem férnek hozzá az Yammer szolgáltatáshoz. További információt a [Yammer felhasználói licencek kezelése az Office 365-ben](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) című témakörben talál. 

Ha a licencek törlődnek a felhasználóktól, a Yammer csempe már nem jelenik meg, és más szolgáltatások is használhatják a licencek eltávolítását a funkciók elrejtéséhez. Egyéb esetekben előfordulhat, hogy a funkciók továbbra is megtalálhatók, de az engedélyek kiosztása működni fog.  

**A licenc nem frissül a felhasználónál**  

Alkalmanként a felhasználó licencet rendel hozzá, de továbbra sem tudja elérni a Yammer. A késések nagyobb valószínűséggel jelentkeznek, ha tömeges licenc-hozzárendelés van folyamatban. Előfordulhat, hogy a Yammer-felhasználók nem frissülnek az Azure AD-ban módosított licencek sorrendjében, mert a rendszer aszinkron módon fut. Várjon akár 24 órát, mielőtt megnyit egy támogatási ügyet a licenc-szinkronizálási problémák bejelentéséhez.  

**Tömeges licenc-hozzárendelés**  

A licencek a felügyeleti központban vagy a PowerShell-parancsfájlok segítségével rendelhetők el. További információt a [licencek hozzárendelése a felhasználókhoz](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) és a [licencek hozzárendelése felhasználói fiókokhoz az Office 365 PowerShell használatával](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell)című témakörben talál. 

A Microsoft ügyfélszolgálata nem nyújt segítséget a parancsfájlok létrehozásához, de a Yammer licenc-hozzárendelés dokumentációja elérhető. További információt a Yammer- [licencek kezelése a Windows PowerShell használatával](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell)című témakörben talál.