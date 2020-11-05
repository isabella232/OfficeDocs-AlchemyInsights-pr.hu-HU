---
title: Modern Azure-alapú levelezés számlázása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003801"
- "6866"
ms.openlocfilehash: 65df6091a97d4937379ded384a78b5d07aa76e42
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922063"
---
# <a name="email-invoicing-in-azure"></a>E-mail-számlázás az Azure-ban

Az e-mail-számla beállításának frissítéséhez tulajdonossal vagy közreműködő szerepkörrel kell rendelkeznie a számlázási profilban vagy annak számlázási fiókjában. Miután kiválasztotta a jogosultságot, minden felhasználó, aki tulajdonossal, közreműködővel, olvasókkal és számla-kezelő szerepkörrel rendelkezik a számlázási profilban, e-mailben megkapja a számláját.

1. Bejelentkezés az [Azure portálra](https://portal.azure.com/)
2. Keressen a **Cost Management + számlázás** lapra.
3. Válassza a bal oldalon a **számlák** lehetőséget, és válassza az **e-mail-számla** lehetőséget a lap tetején.
4. Ha több számlázási profilja is van, válassza ki a számlázási profilt, majd válassza a bekapcsolás **lehetőséget.**

5. Válassza a **frissítés** lehetőséget.
6. Ha több számlázási profilja is van, válassza ki a számlázási profilt, majd válassza a bekapcsolás **lehetőséget.**

Az MCA-vagy MPA-alapú számlázási profilokban a számla-kezelő szerepkör kiosztásával hozzáférést adhat másoknak a számlák megtekintéséhez, letöltéséhez és kifizetéséhez. Ha úgy döntött, hogy a számlát e-mailben kapja meg, a felhasználók a számlákat e-mailben is megkapják.

1. Bejelentkezés az [Azure portálra](https://portal.azure.com/)
2. Keressen a **Cost Management + számlázás** lapra.
3. Válassza a **Számlázási profilok** lehetőséget a bal oldali oldalról. A számlázási profilok listában válassza ki azt a számlázási profilt, amelyhez számlát kezelő szerepkört szeretne rendelni.
4. Kattintson a bal oldalon a **hozzáférés-vezérlés (iam)** elemre, és válassza a lap tetején a **Hozzáadás** lehetőséget.

A szerepkör legördülő listában válassza a számla- **kezelő** lehetőséget. Adja meg annak a felhasználónak az e-mail-címét, akinek hozzáférést szeretne adni. A szerepkör hozzárendeléséhez válassza a **Mentés** gombot.
