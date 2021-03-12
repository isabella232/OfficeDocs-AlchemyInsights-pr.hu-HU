---
title: Feltételes hozzáférés Intune-nal
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 20ef8205431aad821419f2559be3402c8228d838
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704788"
---
# <a name="conditional-access-with-intune"></a>Feltételes hozzáférés Intune-nal

A  **feltételes hozzáférés**  Intune-nal való használatához 3 lépés szükséges:

- Megfelelőségi  **szabályzat** [(Android,](https://docs.microsoft.com/intune/compliance-policy-create-android)  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios)és  [Windows)](https://docs.microsoft.com//intune/compliance-policy-create-windows)segítségével megadhatja azokat a beállításokat, amelyeknek teljesülnie kell ahhoz, hogy az eszköz megfelelőnek minősül. Egy eszköznek például legalább 6 jegyű pin-kódot kell lennie, mielőtt megfelelőnek minősül.
- Hozzon létre **egy feltételes**  hozzáférési házirendet, amely meghatározza, hogy milyen erőforrások vannak védve, és milyen feltételeknek kell teljesülni az erőforrások eléréséhez.  [Egy eszköznek például](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  kompatibilisnek kell lennie a vállalati e-mailek elérése előtt.
- Győződjön meg **arról, hogy a megfelelőségi szabályzatok**  és  **a**  feltételes hozzáférési szabályzatok a kívánt felhasználócsoportokra vannak megcélzottak. Ehhez szükség lehet bizonyos felhasználói csoportok létrehozására az Azure Active Directoryban.

**Hasznos hivatkozások:**

[Eszköz-megfelelőség áttekintése](https://docs.microsoft.com/intune/device-compliance-get-started)

[A hitelesítésszolgáltató hibaelhárítása](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Hibaelhárítási házirend](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

Az e-mailek (Exchange Online) nem kompatibilis eszközök által való elérésének védelme érdekében mindkét dokumentumot követnie kell:

1. [Az e-mailek elérésének védelme az eszközökről az EAS használatával](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Az e-mail-hozzáférés védelme az eszközökről modern hitelesítési ügyfélprogramokkal, például az Outlookkal](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)