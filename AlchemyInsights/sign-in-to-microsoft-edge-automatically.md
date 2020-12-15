---
title: Bejelentkezés a Microsoft Edge-be automatikusan
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
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677765"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Bejelentkezés a Microsoft Edge-be automatikusan

A Microsoft Edge az operációs rendszer alapértelmezett fiókját használva automatikusan bejelentkezik a felhasználókba a felhasználó eszközének beállítása szerint. 

Az egyes eszközök konfigurációjának és a függő felhasználó bejelentkezési folyamatának forgatókönyvei alább olvashatók:

1. **Az eszköz hibrid/aad-J**: Ez a beállítás a Windows 10, a Down-Level Windows és a megfelelő kiszolgálói verziókban érhető el. A felhasználók automatikusan bejelentkeznek az Azure Active Directory (AD) fiókjaival.
2. **Az eszköz tartományhoz csatlakozik**: Ez a beállítás a Windows 10, a Down-Level Windows és a megfelelő kiszolgálói verziókban érhető el. Alapértelmezés szerint a tartományi fiókokkal rendelkező felhasználók nincsenek bejelentkezve automatikusan; Ha engedélyezni szeretné az automatikus bejelentkezést, használja a **ConfigureOnPremisesAccountAutoSignIn** házirendet. Ha engedélyezni szeretné az automatikus bejelentkezést az Azure AD-fiókkal rendelkező felhasználók számára, fontolja meg a hibrid csatlakozást az eszközökhöz.
3. **Az operációs rendszer alapértelmezett fiókja a Microsoft-fiók**: Ez a beállítás a Windows 10 RS3 (1709-es verzió, 10.0.16299-es verzió) és újabb verzióiban érhető el. A forgatókönyv nem valószínű a nagyvállalati eszközökön való előfordulásra. Ha azonban az operációs rendszer alapértelmezett fiókja Microsoft-fiók, a Microsoft Edge automatikusan bejelentkezik a felhasználóhoz a Microsoft-fiókkal.
 
 
