---
title: Hiba történt az asztali adatellenőrzéskor az Access-jogkivonat hibájának érvényesítésekor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783553"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>"Hiba történt az Access-jogkivonat érvényesítése közben" hiba történt az asztali adatelemzés során

Ezt a hibát általában a hitelesítő jogkivonat lejárta után kell megtartani. A lap frissítése általában frissíti a jogkivonatot. Ez a probléma azonban fennmaradhat, ha vannak feltételes hozzáférésű házirendek, amelyeket az asztali számítógép-elemzéshez használt fiókra alkalmaznak. Áttekintheti az Azure AD bejelentkezési naplóit az Azure portálon annak megállapításához, hogy vannak-e bejelentkezési hibák a bevezetéshez használt fiókhoz.

A feltételes hozzáférésről további információt a [feltételes hozzáférés bevezetésének megtervezése](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)című témakörben találhat.