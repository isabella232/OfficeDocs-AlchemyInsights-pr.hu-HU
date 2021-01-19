---
title: Tulajdonossal kapcsolatos problémák elhárítása
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7815"
- "9004358"
ms.openlocfilehash: 914d5682a403197a8569bb75fda8a77449f485f6
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901004"
---
# <a name="troubleshoot-owner-issues"></a>Tulajdonossal kapcsolatos problémák elhárítása

A tulajdonossal kapcsolatos hibák elhárításához végezze el az alábbi lépéseket:

1. [Azure-előfizetések rendszergazdáinak](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners)hozzáadása vagy módosítása: Az Azure Active Directory (Azure AD) csoportokat a csoporttulajdonosok birtokolják és kezelik. A csoporttulajdonosok lehetnek felhasználók vagy egyszerű szolgáltatástulajdonosok, és felügyelni tudják a csoportot, beleértve a tagságot is. Csak a meglévő csoporttulajdonosok és a csoportokat kezelő rendszergazdák rendelhetnek hozzá csoporttulajdonosokat. A csoporttulajdonosoknak nem kell a csoport tagjainak lennie.
2. [Azure-előfizetési](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)rendszergazdák hozzáadása vagy módosítása: Ez a cikk azt ismerteti, hogy miként adhat hozzá vagy módosíthat rendszergazdai szerepkört egy felhasználónál az Azure RBAC használatával az előfizetés hatókörében.
3. A PowerShell-parancsokkal csoport- vagy alkalmazástulajdonost adhat hozzá.
