---
title: Feltételes hozzáférési szabályzatok
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002357"
- "4583"
ms.openlocfilehash: a518d70f03f3034a60f0c9ded40ee6ab5140a5163021337c3a2aee7f18575c3d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54033712"
---
# <a name="conditional-access-policies"></a>Feltételes hozzáférési szabályzatok

A feltételes hozzáférés az Azure AD funkciója, amely lehetővé teszi a vezérlők kényszerítését a környezetében lévő appokhoz való hozzáféréshez, adott feltételek alapján és egy központi helyről felügyelve.

További információ az [Azure AD feltételes hozzáférés](https://docs.microsoft.com/azure/active-directory/conditional-access/) funkciójáról.  

**Megjegyzés**: Ha bérlői fiókját 2019. október 21. után hozták létre, és Önt váratlanul többtényezős hitelesítésre kérik, akkor a bérlői fiókban valószínűleg engedélyezték az [alapértelmezett biztonsági beállításokat](https://aka.ms/securitydefaults).

**Az alapértelmezett biztonsági beállítások kezelése**

1. Jelentkezzen be a [felügyeleti központba](https://go.microsoft.com/fwlink/p/?linkid=834822) a globális rendszergazdai hitelesítő adataival.

2. Lépjen az [Azure Active Directory – Tulajdonságok](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties) lapra.

3. A lap alján válassza ki az **Alapértelmezett biztonsági beállítások kezelése** lehetőséget.

4. Válassza az **Igen** lehetőséget a biztonsági alapértékek engedélyezéséhez, és a **Nem** lehetőséget a biztonsági alapértékek letiltásához.
