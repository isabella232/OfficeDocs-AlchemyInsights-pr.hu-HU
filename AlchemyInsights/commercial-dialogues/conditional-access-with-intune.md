---
title: A feltételes hozzáférés használata az Intune-nal
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 23afea21668191093d612d68ca6e9ab2a844f4a14977631d33f4fd956fc3c4e7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005776"
---
# <a name="using-conditional-access-with-intune"></a>A feltételes hozzáférés használata az Intune-nal

A feltételes hozzáférés Intune-nal való használata 3 lépést igényel:

- [Hozzon létre egy megfelelőségi szabályzatot, amely meghatározza azokat a beállításokat, amelyeknek meg kell felelnie ahhoz, hogy az eszköz megfelelőnek minősül. Egy eszköznek például legalább 6 számjegyű PIN-kódot kell kitűznie, mielőtt megfelelőnek minősül.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Hozzon létre egy feltételes hozzáférési házirendet, amely meghatározza a védett erőforrásokat és az erőforrások eléréséhez szükséges feltételeket. Egy eszköznek például kompatibilisnek kell lennie a vállalati e-mailek elérése előtt.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Győződjön meg arról, hogy a megfelelőségi szabályzatok és a feltételes hozzáférési szabályzatok a kívánt felhasználócsoportokra vannak megcélzottak. Ehhez szükség lehet adott felhasználócsoportok létrehozására a Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[További tudnivalók...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
