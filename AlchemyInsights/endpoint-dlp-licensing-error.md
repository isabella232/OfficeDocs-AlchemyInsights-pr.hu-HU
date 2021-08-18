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
ms.openlocfilehash: c32ab88a72c265be411350e50756f5b2e1e3337c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58322133"
---
# <a name="endpoint-dlp-licensing-error"></a>Endpoint DLP Licensing error

Az Endpoint DLP beállításakor a következő hibaüzenet jelenik meg:

`Your organization is missing the licenses required to manage these devices`.

Győződjön meg arról, hogy az alábbi előfizetések vagy bővítmények valamelyikével rendelkezik:

- Microsoft 365 E5
- Microsoft 365 A5 csomag (EDU)
- Microsoft 365 E5 megfelelőség
- Microsoft 365 A5 csomag megfelelőség
- Microsoft 365 E5 információvédelem és -szabályozás
- Microsoft 365 A5 csomag információvédelem és -szabályozás

**Megjegyzés:** Ez nem működik licenckombinációk esetén, például: Win E5 + O365 E5 + EMS E5. A funkció beállításához csak M365 E5 licenccel kell rendelkezik.

Az Endpoint DLP licencelési információiról az [Endpoint DLP licensing (Végponti DLP-licencelés) témakörben található.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
