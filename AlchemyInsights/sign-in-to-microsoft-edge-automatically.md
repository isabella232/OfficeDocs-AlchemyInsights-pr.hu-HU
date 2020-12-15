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
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="f701f-102">Bejelentkezés a Microsoft Edge-be automatikusan</span><span class="sxs-lookup"><span data-stu-id="f701f-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="f701f-103">A Microsoft Edge az operációs rendszer alapértelmezett fiókját használva automatikusan bejelentkezik a felhasználókba a felhasználó eszközének beállítása szerint.</span><span class="sxs-lookup"><span data-stu-id="f701f-103">Microsoft Edge uses the OS's default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="f701f-104">Az egyes eszközök konfigurációjának és a függő felhasználó bejelentkezési folyamatának forgatókönyvei alább olvashatók:</span><span class="sxs-lookup"><span data-stu-id="f701f-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

1. <span data-ttu-id="f701f-105">**Az eszköz hibrid/aad-J**: Ez a beállítás a Windows 10, a Down-Level Windows és a megfelelő kiszolgálói verziókban érhető el.</span><span class="sxs-lookup"><span data-stu-id="f701f-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="f701f-106">A felhasználók automatikusan bejelentkeznek az Azure Active Directory (AD) fiókjaival.</span><span class="sxs-lookup"><span data-stu-id="f701f-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
2. <span data-ttu-id="f701f-107">**Az eszköz tartományhoz csatlakozik**: Ez a beállítás a Windows 10, a Down-Level Windows és a megfelelő kiszolgálói verziókban érhető el.</span><span class="sxs-lookup"><span data-stu-id="f701f-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="f701f-108">Alapértelmezés szerint a tartományi fiókokkal rendelkező felhasználók nincsenek bejelentkezve automatikusan; Ha engedélyezni szeretné az automatikus bejelentkezést, használja a **ConfigureOnPremisesAccountAutoSignIn** házirendet.</span><span class="sxs-lookup"><span data-stu-id="f701f-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="f701f-109">Ha engedélyezni szeretné az automatikus bejelentkezést az Azure AD-fiókkal rendelkező felhasználók számára, fontolja meg a hibrid csatlakozást az eszközökhöz.</span><span class="sxs-lookup"><span data-stu-id="f701f-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
3. <span data-ttu-id="f701f-110">**Az operációs rendszer alapértelmezett fiókja a Microsoft-fiók**: Ez a beállítás a Windows 10 RS3 (1709-es verzió, 10.0.16299-es verzió) és újabb verzióiban érhető el.</span><span class="sxs-lookup"><span data-stu-id="f701f-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="f701f-111">A forgatókönyv nem valószínű a nagyvállalati eszközökön való előfordulásra.</span><span class="sxs-lookup"><span data-stu-id="f701f-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="f701f-112">Ha azonban az operációs rendszer alapértelmezett fiókja Microsoft-fiók, a Microsoft Edge automatikusan bejelentkezik a felhasználóhoz a Microsoft-fiókkal.</span><span class="sxs-lookup"><span data-stu-id="f701f-112">However, if the OS's default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
