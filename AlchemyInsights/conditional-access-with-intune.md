---
title: Feltételes hozzáférés a Intune szolgáltatással
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807661"
---
# <a name="conditional-access-with-intune"></a>Feltételes hozzáférés a Intune szolgáltatással

A  **feltételes hozzáférés**  használata a Intune használatához 3 lépésből áll:

- Hozzon létre egy  **megfelelőségi házirendet**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) a megfelelő beállítások megadásához, mielőtt az eszköz megfelel-e a követelményeknek. Az eszközöknek például legalább 6 számjegyből álló PIN-kóddal kell rendelkezniük ahhoz, hogy megfeleljenek a megfelelőségi követelményeknek.
- Hozzon létre egy **feltételes hozzáférési házirendet**  , amely meghatározza, hogy milyen erőforrások legyenek védve, és milyen feltételeknek kell teljesülniük ahhoz, hogy hozzáférhessenek ezekhez az erőforrásokhoz.  [Az](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  eszközöknek például kompatibiliseknek kell lenniük a vállalati e-mailek eléréséhez.
- Gondoskodjon arról, hogy a **megfelelőségi szabályok**  és a  **feltételes hozzáférés-házirendek**  a felhasználók kívánt csoportjaira irányuljanak. Ehhez szükség lehet az Azure Active Directory-beli felhasználók bizonyos csoportjai létrehozására.

**Hasznos hivatkozások:**

[Az eszközök megfelelősége – áttekintés](https://docs.microsoft.com/intune/device-compliance-get-started)

[HITELESÍTÉSSZOLGÁLTATÓ hibaelhárítása](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Hibaelhárítási szabályok](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

Ha nem kompatibilis eszközökről szeretné megvédeni az e-maileket (Exchange Online), mindkét dokumentumot meg kell tartani:

1. [E-mail-hozzáférés védelme az eszközökről az EAS segítségével](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [E-mail-hozzáférés biztosítása az eszközökről a modern hitelesítési ügyfélprogramokkal (például az Outlookkal)](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)