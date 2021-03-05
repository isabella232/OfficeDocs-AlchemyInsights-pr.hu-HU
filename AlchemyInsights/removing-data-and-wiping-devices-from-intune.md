---
title: Adatok eltávolítása és eszközök tartalmának törlése az Intune-ból
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
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416315"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Adatok eltávolítása és eszközök tartalmának törlése az Intune-ból

Az Eszköz kivezetése és az Eszköz adatainak törlése távoli művelettel eltávolíthatja az Intune által kezelt céges adatokat, illetve gyári alaphelyzetbe állítást végezhet, és visszaállíthatja az eszköz alapértelmezett beállításait.

1. Jelentkezzen be a Microsoft 365 Eszközkezelés szolgáltatásba, és válassza az **Eszközök** > **Az összes eszköz** lehetőséget.
2. Válassza ki az eszközt, amelyről törölni szeretné az adatokat.
3. Válassza ki a végrehajtandó távoli törlés típusát. A kivezetés csak a szervezeti adatokat törli, míg a teljes törlés visszaállítja az eszköz gyári beállításait.
4. Az **Igen** gombot választva erősítse meg a műveletet. A törlés befejeződéséig az Eszközművelet állapota *Megszüntetés függőben* lesz.
    A művelet befejeződését követően a mobileszköz többé nem lesz látható a felügyelt eszközök listáján.

> [!NOTE]
> A céges adatok nem távolíthatók el az Azure AD-hez csatlakoztatott eszközökről. 

A kivezetési és törlési műveletek hatásairól az alábbi dokumentációban talál részletes tájékoztatást, egyebek között a megőrzött és a törölt adatok ismertetését:

- [Eszközök eltávolítása adattörléssel, kivezetéssel vagy a regisztrációjuk manuális megszüntetésével](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe)
- [Csak a vállalati adatok törlése az Intune által kezelt alkalmazásokból](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [Az összes adat törlése macOS rendszerű eszközről](https://docs.microsoft.com/mem/intune/remote-actions/device-erase)