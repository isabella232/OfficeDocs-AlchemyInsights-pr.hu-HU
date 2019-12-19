---
title: Hiba történt a hozzáférési token hibának érvényesítésekor az asztali Analytics on-Board
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741196"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>"Hiba történt a hozzáférési token érvényesítése közben" hiba történt az asztali Analytics felkészítése

Ezt a hibát általában a hitelesítési jogkivonat lejártakor kell betartani. Az oldal frissítése általában frissíti a jogkivonatot. Azonban ez a probléma akkor is fennállhat, ha a Desktop Analytics fedélzetén használt fiókra feltételes hozzáférési házirendek vannak alkalmazva. Az Azure Portal webhelyen található Azure AD bejelentkezési naplókból megtekintheti, hogy vannak-e bejelentkezési hibák az asztali Analyticshez használt fiók esetében.

Ha többet szeretne megtudni a feltételes elérésről, látogasson el [a feltételes hozzáférésű telepítés tervbe](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).