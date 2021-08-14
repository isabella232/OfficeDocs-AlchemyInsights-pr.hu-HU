---
title: 'Az Android Enterprise regisztrációs hibája: Az MGP beállítás észlelése'
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000652"
- "8340"
ms.openlocfilehash: 9493d4cede39b4fb5aa41638c0f709b9025b2468ade322be6991bdad17e97d5d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932855"
---
# <a name="android-enterprise-enrollment-error-mgp-set-up-detection"></a>Az Android Enterprise regisztrációs hibája: Az MGP beállítás észlelése

Azt észleltük, hogy a Felügyelt Google Play nincs beállítva vagy leválasztva a fiókjához. Ez problémákat okozhat az androidos nagyvállalati eszközök beléptetésében olyan esetekben, ahol Felügyelt Google Play kapcsolat szükséges.

A Felügyelt Google Play szolgáltatás kapcsolati állapotát a MeM konzol Bérlő felügyelete > **Tenant status > Connector status** (Bérlői fiók állapota > Összekötő állapota) területén ellenőrizheti, és az Intune-fiók Felügyelt Google-fiókhoz való csatlakoztatásának mikéntjéhez megismerheti az Intune Csatlakozás-fiókját a Felügyelt Google Play-fiókkal. **[](https://docs.microsoft.com/mem/intune/enrollment/connect-intune-android-enterprise)**
