---
title: Végponti DLP licencelési hiba
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
ms.openlocfilehash: d17c51177898d62c7c477460c8c26b4753bae65f
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564610"
---
# <a name="endpoint-dlp-licensing-error"></a>Végponti DLP licencelési hiba

Ha a következőhöz hasonló hibaüzenet jelenik meg, amikor megkísérli beállítani a Endpoint DLP-t, a következő hibaüzenet jelenik meg:

`Your organization is missing the licenses required to manage these devices`.

Ellenőrizze, hogy rendelkezik-e az alábbi előfizetések vagy bővítmények egyikével:

- Microsoft 365 E5
- Microsoft 365 a5 (EDU)
- Microsoft 365 E5 megfelelőség
- Microsoft 365 a5 megfelelőség
- Microsoft 365 E5 – adatvédelem és irányítás
- Microsoft 365 a5 – adatvédelem és irányítás

> [!NOTE]
> Ez a funkció nem működik a licenc-kombinációk esetében, például: Win E5 + O365 E5 + EMS E5. A funkció beállításához rendelkeznie kell egy tisztán M365 E5 licenccel.

További Végpontos DLP-licencelési információkért lásd: [ENDPOINT DLP Licensing.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
