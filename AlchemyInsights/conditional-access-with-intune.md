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
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931434"
---
# <a name="conditional-access-with-intune"></a>Feltételes hozzáférés az Intune-nal

A **feltételes hozzáférés** intune-nal való használata 3 lépést igényel:

- Hozzon létre **megfelelőségi szabályzatot** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) olyan beállítások meghatározásához, amelyeknek meg kell felelniük ahhoz, hogy az eszköz megfelelőnek minősüljen. Egy eszköznek például legalább 6 számjegyből álló tűvel kell rendelkeznie ahhoz, hogy megfelelőnek minősüljön.
- Hozzon létre egy **feltételes hozzáférési szabályzatot,** amely meghatározza, hogy milyen erőforrások at védenek, és milyen feltételeknek kell megfelelni az erőforrások eléréséhez.  Egy eszköznek [például](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) megfelelőnek kell lennie a vállalati e-mailek elérése előtt.
- Győződjön meg arról, hogy mind **a megfelelőségi szabályzatok,** mind a **feltételes hozzáférési házirendek** a kívánt felhasználói csoportokat célozzák meg. Ez szükség lehet a felhasználók adott csoportjainak az Azure Active Directoryban.

**Hasznos linkek:**

[Eszközmegfelelőség – áttekintés](https://docs.microsoft.com/intune/device-compliance-get-started)

[Hitelesítésak – hibaelhárítás](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Hibaelhárítási házirend](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

Annak érdekében, hogy az e-maileket (Exchange online) megvédje a nem megfelelő eszközök hozzáférésétől, mindkét dokumentumot be kell tartani:

1. [Az e-mailek elérésének védelme az eszközökről az EAS használatával](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Az e-mailek elérésének védelme az eszközökkel a modern hitelesítési ügyfelek, például az Outlook használatával](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)