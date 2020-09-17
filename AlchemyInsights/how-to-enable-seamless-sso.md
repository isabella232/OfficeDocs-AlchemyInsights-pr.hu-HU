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
# <a name="how-to-enable-seamless-sso"></a>A zökkenőmentes egyszeri bejelentkezés engedélyezése

Engedélyezze a zökkenőmentes egyszeri bejelentkezést az [Azure ad Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect)segítségével.
  
Ha az Azure AD Connect új példányát használja, válassza az [egyéni telepítési útvonalat](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom). A **felhasználói bejelentkezési** lapon jelölje be az **egyszeri bejelentkezés engedélyezése** jelölőnégyzetet.
  
Annak ellenőrzése, hogy helyesen engedélyezte-e a zökkenőmentes egyszeri bejelentkezést:
  
1. Bejelentkezés az [Azure Active Directory felügyeleti központba](https://aad.portal.azure.com) globális rendszergazdaként.

2. Válassza az **Azure Active Directory** lehetőséget a bal oldali ablaktáblában.

3. Ellenőrizze, hogy **engedélyezve**van-e a zökkenőmentes egyszeri bejelentkezés.

További információt az [Azure Active Directory zökkenőmentes egyszeri bejelentkezés: rövid útmutató](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start)című témakörben talál.
  