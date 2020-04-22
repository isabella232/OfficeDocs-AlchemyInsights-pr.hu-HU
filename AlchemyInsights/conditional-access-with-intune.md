---
title: Feltételes hozzáférés az Intune-nal
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c9c47d71b2da3840504d5b28c7c9e067b4c05fa5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706023"
---
# <a name="conditional-access-with-intune"></a>Feltételes hozzáférés az Intune-nal

A **feltételes hozzáférés** intune-nal való használata 3 lépést igényel: 
  
- Hozzon létre egy **feltételes hozzáférési szabályzatot,** amely meghatározza, hogy milyen erőforrások at védenek, és milyen feltételeknek kell megfelelni az erőforrások eléréséhez. Egy eszköznek például megfelelőnek kell lennie a vállalati e-mailek elérése előtt. 
    
- Hozzon létre egy **megfelelőségi szabályzatot** olyan beállítások meghatározásához, amelyeket teljesíteni kell ahhoz, hogy az eszköz megfelelőnek minősüljen. Egy eszköznek például legalább 6 számjegyből álló tűvel kell rendelkeznie ahhoz, hogy megfelelőnek minősüljön. 
    
- Annak **biztosítása, hogy mind a megfelelőségi szabályzatok,** mind a **feltételes hozzáférési házirendek** a kívánt felhasználói csoportokra irányuljanak. Ez szükség lehet a felhasználók adott csoportjainak az Azure Active Directoryban. 
    
Bővebben:
  
- [A feltételes hozzáféréssel kapcsolatos gyakorlati tanácsok](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [A feltételes hozzáférés – első lépések](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

