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
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="22019-102">Automatikus bejelentkezés a Microsoft Edge-be</span><span class="sxs-lookup"><span data-stu-id="22019-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="22019-103">A Microsoft Edge az operációs rendszer alapértelmezett fiókjával jelentkeztet be automatikusan egy felhasználót a felhasználó eszközének konfigurációja szerint.</span><span class="sxs-lookup"><span data-stu-id="22019-103">Microsoft Edge uses the OS default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="22019-104">Az egyes eszközkonfigurációk és a függő felhasználói bejelentkezési folyamat forgatókönyvei az alábbiak:</span><span class="sxs-lookup"><span data-stu-id="22019-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

- <span data-ttu-id="22019-105">**Az eszköz hibrid/AAD-J:** Ez a beállítás a Windows 10-es és a windowsos verziókban, valamint a kiszolgáló megfelelő verzióiban érhető el.</span><span class="sxs-lookup"><span data-stu-id="22019-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="22019-106">A felhasználók automatikusan bejelentkeznek Azure Active Directory-(AD) fiókjukkal.</span><span class="sxs-lookup"><span data-stu-id="22019-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
- <span data-ttu-id="22019-107">**Az eszköz tartományhoz van stb.:** Ez a lehetőség Windows 10-es, lefelé és kiszolgálói verziókban érhető el.</span><span class="sxs-lookup"><span data-stu-id="22019-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="22019-108">A tartományi fiókkal rendelkező felhasználók alapértelmezés szerint nem jelentkeznek be automatikusan; Az automatikus bejelentkezés engedélyezéséhez használja a **ConfigureOnPremisesAccountAutoSignIn házirendet.**</span><span class="sxs-lookup"><span data-stu-id="22019-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="22019-109">Ha engedélyezni szeretné az automatikus bejelentkezést az Azure AD-fiókkal rendelkező felhasználók számára, fontolja meg az eszközök hibrid csatlakozását.</span><span class="sxs-lookup"><span data-stu-id="22019-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
- <span data-ttu-id="22019-110">**Az operációs rendszer** alapértelmezett fiókja egy Microsoft-fiók: Ez a beállítás a Windows 10 RS3 (1709-es verzió, 10.0.16299-es build) és az újabb verziókban érhető el.</span><span class="sxs-lookup"><span data-stu-id="22019-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="22019-111">Ez a helyzet valószínűtlen nagyvállalati eszközökön.</span><span class="sxs-lookup"><span data-stu-id="22019-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="22019-112">Ha azonban az operációs rendszer alapértelmezett fiókja egy Microsoft-fiók, akkor a Microsoft Edge automatikusan bejelentkezik a felhasználóba a Microsoft-fiókkal.</span><span class="sxs-lookup"><span data-stu-id="22019-112">However, if the OS default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
