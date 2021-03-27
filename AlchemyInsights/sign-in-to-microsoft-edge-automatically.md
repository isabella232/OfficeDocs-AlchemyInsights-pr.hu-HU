---
title: Automatikus bejelentkezés a Microsoft Edge-be
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
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398731"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Automatikus bejelentkezés a Microsoft Edge-be

A Microsoft Edge az operációs rendszer alapértelmezett fiókjával jelentkeztet be automatikusan egy felhasználót a felhasználó eszközének konfigurációja szerint. 

Az egyes eszközkonfigurációk és a függő felhasználói bejelentkezési folyamat forgatókönyvei az alábbiak:

- **Az eszköz hibrid/AAD-J:** Ez a beállítás a Windows 10-es és a windowsos verziókban, valamint a kiszolgáló megfelelő verzióiban érhető el. A felhasználók automatikusan bejelentkeznek Azure Active Directory-(AD) fiókjukkal.
- **Az eszköz tartományhoz van stb.:** Ez a lehetőség Windows 10-es, lefelé és kiszolgálói verziókban érhető el. A tartományi fiókkal rendelkező felhasználók alapértelmezés szerint nem jelentkeznek be automatikusan; Az automatikus bejelentkezés engedélyezéséhez használja a **ConfigureOnPremisesAccountAutoSignIn házirendet.** Ha engedélyezni szeretné az automatikus bejelentkezést az Azure AD-fiókkal rendelkező felhasználók számára, fontolja meg az eszközök hibrid csatlakozását.
- **Az operációs rendszer** alapértelmezett fiókja egy Microsoft-fiók: Ez a beállítás a Windows 10 RS3 (1709-es verzió, 10.0.16299-es build) és az újabb verziókban érhető el. Ez a helyzet valószínűtlen nagyvállalati eszközökön. Ha azonban az operációs rendszer alapértelmezett fiókja egy Microsoft-fiók, akkor a Microsoft Edge automatikusan bejelentkezik a felhasználóba a Microsoft-fiókkal.
 
 
