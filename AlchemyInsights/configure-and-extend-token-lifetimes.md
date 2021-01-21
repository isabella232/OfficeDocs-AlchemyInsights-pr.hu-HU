---
title: A jogkivonat élettartamának konfigurálása és meghosszabbítása
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/20/2021
ms.locfileid: "49916828"
---
# <a name="configure-and-extend-token-lifetimes"></a>A jogkivonat élettartamának konfigurálása és meghosszabbítása

Megadhatja a Microsoft identitásplatform által kibocsátott hozzáférési, SAML- vagy azonosítótokens élettartamát. Beállíthatja a jogkivonat élettartamát a szervezet összes appja, egy több-bérlős (több szervezetből álló) alkalmazás vagy egy adott szolgáltatásnév számára a szervezetben. További információért olvassa el a [konfigurálható jogkivonat élettartamát.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)

Példákat [a jogkivonat élettartamának beállítására vonatkozó példákban talál.](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes)

Ha tudni szeretne arról, hogy miként konfigurálhatja egy jogkivonat élettartamát és kompatibilitását az Azure Active Directory B2C szolgáltatásban (Azure AD B2C), olvassa el a Jogkivonatok konfigurálása az [Azure Active Directory B2C szolgáltatásban.](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow)

A munkamenet viselkedésének konfigurálása az [Azure Active Directory B2C-ben](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) az Azure AD B2C-ben használt egyszeri bejelentkezési módszereket ismerteti, és segít a házirend konfigurálásához a legmegfelelőbb egyszeri bejelentkezési módszer választásában.

**Mennyi ideig tart a jogkivonat? Mennyi ideig érvényesek?**

A tokenek élettartama 1 óra, a munkamenet élettartama pedig 24 óra. Ez azt jelenti, hogy ha 24 órán belül nem történt kérés, újra be kell jelentkeznie, mielőtt új jogkivonatot kér.

> [!NOTE]
> 2020. május 30. után egy új bérlő sem fogja tudni használni a konfigurálható tokenek élettartam-házirendet a munkamenet és a tokenek frissítéséhez. A felállás néhány hónapon belül megtörténik, ami azt jelenti, hogy a meglévő munkamenetet nem fogjuk tiszteletben hagyni, és frissítjük a jogkivonat-rendszerrendeket. A lejárat után is konfigurálhatja a hozzáférési jogkivonat élettartamát.






