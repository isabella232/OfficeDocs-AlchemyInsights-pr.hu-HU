---
title: Üzenettitkosítás konfigurálása hibrid környezetben
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 22c2468b7639680b447b6464431a79b69f7198c3
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524828"
---
# <a name="configure-message-encryption-for-a-hybrid-environment"></a>Üzenettitkosítás konfigurálása hibrid környezetben

Hibrid Exchange-környezetekben a helyszíni felhasználók csak akkor küldhetnek titkosított e-maileket az Office Üzenettitkosítás (OME) használatával, ha az e-maileket az Exchange Online-on keresztül irányítják át.

Az OME használatával az alábbi lépésekkel titkosíthatja az e-maileket:

1. A Hibrid [konfiguráció varázslóval](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) beállíthatja a hibrid környezetet. A titkosítás beállításához nincs szükség speciális lépésekre.
2. A szokásos módon állítsa be az [e-mail-forgalom](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) szabályait titkosításra.


