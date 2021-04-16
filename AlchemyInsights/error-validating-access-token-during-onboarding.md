---
title: Hiba történt a hozzáférési jogkivonat érvényességének érvényességének igazolása közben a telepítés során.
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813690"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>"Hiba történt a hozzáférési jogkivonat érvényességének érvényességének igazolása" hibaüzenet jelenik meg az asztali analytics telepítésének közben

Ez a hiba általában a hitelesítési jogkivonat elévülésekor jelenik meg. A lap frissítése általában frissíti a jogkivonatot. A probléma azonban megmaradhat, ha a táblán található asztali elemzésekhez használt fiókra feltételes hozzáféréssel kapcsolatos házirendek vannak alkalmazva. Az Azure AD bejelentkezési naplóit az Azure Portalon áttekintve ellenőrizze, hogy nem jelentkeznek-e be az asztali elemzésekhez használt fiókhoz.

A feltételes hozzáférésről további információt A feltételes hozzáférés [üzembe helyezésének megterve.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)