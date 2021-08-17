---
title: Bejelentkezés az Microsoft Edge be
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
- "8333"
- "9004625"
ms.openlocfilehash: 4e069a1c75caabf3bef7387140edd5650cf966856b888b5c6b5618a603986d6d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050696"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Bejelentkezés az Microsoft Edge be

Microsoft Edge az operációs rendszer alapértelmezett fiókjával jelentkeztet be automatikusan egy felhasználót a felhasználó eszközének beállításai szerint. 

Az egyes eszközkonfigurációk és a függő felhasználói bejelentkezési folyamat forgatókönyvei az alábbiak:

- **Az eszköz hibrid/AAD-J:** Ez a lehetőség csak Windows 10, lefelé Windows kiszolgálói verziókban érhető el. A felhasználók automatikusan bejelentkeznek a saját Azure Active Directory (AD) fiókjukkal.
- **Az eszköz tartományhoz van stb.:** Ez a beállítás csak Windows 10, lefelé Windows és a kiszolgáló megfelelő verzióiban érhető el. A tartományi fiókkal rendelkező felhasználók alapértelmezés szerint nem jelentkeznek be automatikusan; Az automatikus bejelentkezés engedélyezéséhez használja a **ConfigureOnPremisesAccountAutoSignIn házirendet.** Ha engedélyezni szeretné az automatikus bejelentkezést az Azure AD-fiókkal rendelkező felhasználók számára, fontolja meg az eszközök hibrid csatlakozását.
- **Az operációs rendszer** alapértelmezett fiókja egy Microsoft-fiók: Ez a beállítás a Windows 10 RS3 (1709-es verzió, 10.0.16299-es build) és újabb verziókban érhető el. Ez a helyzet valószínűtlen nagyvállalati eszközökön. Ha azonban az operációs rendszer alapértelmezett fiókja egy Microsoft-fiók, akkor Microsoft Edge jelentkezik be a felhasználóba a Microsoft-fiókkal.
 
 
