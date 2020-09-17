---
title: A zökkenőmentes egyszeri bejelentkezés engedélyezése
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
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: f3581549823e1ec650a3717780bc07e9944d4c1c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780529"
---
# <a name="how-to-enable-seamless-sso"></a><span data-ttu-id="09cea-102">A zökkenőmentes egyszeri bejelentkezés engedélyezése</span><span class="sxs-lookup"><span data-stu-id="09cea-102">How to enable Seamless SSO</span></span>

<span data-ttu-id="09cea-103">Engedélyezze a zökkenőmentes egyszeri bejelentkezést az [Azure ad Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect)segítségével.</span><span class="sxs-lookup"><span data-stu-id="09cea-103">Enable Seamless SSO through [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span></span>
  
<span data-ttu-id="09cea-104">Ha az Azure AD Connect új példányát használja, válassza az [egyéni telepítési útvonalat](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span><span class="sxs-lookup"><span data-stu-id="09cea-104">If you're doing a fresh installation of Azure AD Connect, choose the [custom installation path](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span></span> <span data-ttu-id="09cea-105">A **felhasználói bejelentkezési** lapon jelölje be az **egyszeri bejelentkezés engedélyezése** jelölőnégyzetet.</span><span class="sxs-lookup"><span data-stu-id="09cea-105">At the **User sign-in** page, choose the **Enable single sign-on** option.</span></span>
  
<span data-ttu-id="09cea-106">Annak ellenőrzése, hogy helyesen engedélyezte-e a zökkenőmentes egyszeri bejelentkezést:</span><span class="sxs-lookup"><span data-stu-id="09cea-106">To verify that you have enabled Seamless SSO correctly:</span></span>
  
1. <span data-ttu-id="09cea-107">Bejelentkezés az [Azure Active Directory felügyeleti központba](https://aad.portal.azure.com) globális rendszergazdaként.</span><span class="sxs-lookup"><span data-stu-id="09cea-107">Sign in to the [Azure Active Directory administrative center](https://aad.portal.azure.com) as a global admin.</span></span>

2. <span data-ttu-id="09cea-108">Válassza az **Azure Active Directory** lehetőséget a bal oldali ablaktáblában.</span><span class="sxs-lookup"><span data-stu-id="09cea-108">Select **Azure Active Directory** in the left pane.</span></span>

3. <span data-ttu-id="09cea-109">Ellenőrizze, hogy **engedélyezve**van-e a zökkenőmentes egyszeri bejelentkezés.</span><span class="sxs-lookup"><span data-stu-id="09cea-109">Verify that Seamless single sign-on is **Enabled**.</span></span>

<span data-ttu-id="09cea-110">További információt az [Azure Active Directory zökkenőmentes egyszeri bejelentkezés: rövid útmutató](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="09cea-110">To learn more, see [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span></span>
  