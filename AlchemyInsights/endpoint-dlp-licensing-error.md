---
title: Endpoint DLP licensing error
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200001"
- "7176"
ms.openlocfilehash: 1e242abe18717e5ef64d6f067ab3ec6fa8833cb672dd21c85e577ce640240ba0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090144"
---
# <a name="endpoint-dlp-licensing-error"></a>Endpoint DLP Licensing error

Az Endpoint DLP beállításakor az alábbi hibaüzenet jelenik meg:

`Your organization is missing the licenses required to manage these devices`.

Győződjön meg arról, hogy az alábbi előfizetések vagy bővítmények valamelyikével rendelkezik:

- Microsoft 365 E5
- Microsoft 365 A5 csomag (EDU)
- Microsoft 365 E5 megfelelőség
- Microsoft 365 A5 csomag megfelelőség
- Microsoft 365 E5 információvédelem és -szabályozás
- Microsoft 365 A5 csomag információvédelem és -szabályozás

> [!NOTE]
> Ez nem működik licenckombinációk esetén, például: Win E5 + O365 E5 + EMS E5. A funkció beállításához csak M365 E5 licenccel kell rendelkezik.

Az Endpoint DLP licencelési információiról az [Endpoint DLP licensing (VégpontI DLP-licencelés) témakörben található.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
