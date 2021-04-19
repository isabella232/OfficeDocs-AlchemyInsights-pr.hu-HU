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
ms.openlocfilehash: af95627d07d41add54f03c9254562b9be4e05d9b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817282"
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
