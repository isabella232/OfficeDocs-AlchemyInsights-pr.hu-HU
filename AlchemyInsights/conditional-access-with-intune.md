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
ms.openlocfilehash: c24451fba8b8ab8fe7a1778bb292dec6678e1ef487076d27458c9aeb4963c683
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069714"
---
# <a name="conditional-access-with-intune"></a>Feltételes hozzáférés Intune-nal

A  **feltételes hozzáférés**  Intune-nal való használata 3 lépést igényel:

- Hozzon létre egy megfelelőségi **szabályzatot** [(Android,](https://docs.microsoft.com/intune/compliance-policy-create-android) [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios)vagy [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)), és adja meg azokat a beállításokat, amelyeknek teljesülnie kell ahhoz, hogy az eszköz megfelelőnek minősül. Egy eszköznek például legalább 6 számjegyű PIN-kódot kell kitűznie, mielőtt megfelelőnek minősül.
- Hozzon létre **egy feltételes hozzáférési**  házirendet, amely meghatározza a védett erőforrásokat és az erőforrások eléréséhez szükséges feltételeket.  [Egy eszköznek például](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  kompatibilisnek kell lennie a vállalati e-mailek elérése előtt.
- Győződjön meg arról, hogy a megfelelőségi **szabályzatok**  és  **a**  feltételes hozzáférési szabályzatok a kívánt felhasználócsoportokra vannak megcélzottak. Ehhez szükség lehet adott felhasználócsoportok létrehozására a Azure Active Directory.

**Hasznos hivatkozások:**

[Eszközök megfelelősége – áttekintés](https://docs.microsoft.com/intune/device-compliance-get-started)

[Hitelesítésszolgáltató hibaelhárítása](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Hibaelhárítási házirend](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

Az e-mailek (Exchange) nem kompatibilis eszközök által való elérésének védelméhez mindkét dokumentumot be kell tartani:

1. [EAS-hozzáférés védelme az eszközökről](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [E-mail-hozzáférés védelme az eszközökről modern hitelesítési ügyfélprogramokkal (például Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)