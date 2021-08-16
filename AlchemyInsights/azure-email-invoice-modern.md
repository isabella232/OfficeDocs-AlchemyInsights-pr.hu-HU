---
title: Modern Azure e-mailes számlázás
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
- "9003801"
- "6866"
ms.openlocfilehash: caf300873c3a9a97502819c7938ecc86491795d2fc7b6f022ead5d38ca965b8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082836"
---
# <a name="email-invoicing-in-azure"></a>E-mailes számlázás az Azure-ban

Az e-mailben beállított számla preferencia frissítéséhez tulajdonosi vagy közreműködői szerepkörrel kell lennie a számlázási profilban vagy a számlázási fiókban. Miután regisztrált, a számlázási profilhoz tulajdonosi, közreműködői, olvasói, valamint számlakezelői szerepkörrel rendelkező valamennyi felhasználó e-mailben fogja megkapni a számláját.

1. Jelentkezzen be az [Azure portálra](https://portal.azure.com/).
2. Keresse meg a **Költségkezelés + számlázás** elemet.
3. Válassza a **Számlák** lehetőséget a bal oldalon, és válassza a **Számla küldése e-mailben** lehetőséget az oldal tetején.
4. Ha több számlázási profillal rendelkezik, válasszon ki egyet, majd a **Jóváhagyás** lehetőséget.

5. Válassza a **Frissítés** lehetőséget.
6. Ha több számlázási profillal rendelkezik, válasszon ki egyet, majd a **Jóváhagyás** lehetőséget.

Hozzáférést ad másoknak a számlák megtekintéséhez, letöltéséhez és kifizetéséhez, ha egy MCA- vagy MPA-számlázási profilhoz társítja nekik a számlakezelői szerepkört. Ha úgy dönt, hogy e-mailben kapja meg a számlát, a felhasználók is e-mailben kapják meg.

1. Jelentkezzen be az [Azure portálra](https://portal.azure.com/).
2. Keresse meg a **Költségkezelés + számlázás** elemet.
3. Válassza a **Számlázási profilok** opciót a bal oldalon. A számlázási profilok listájában válassza ki azt a számlázási profilt, amelyhez számlakezelői szerepkört szeretne rendelni.
4. Válassza a **Hozzáférés-vezérlés (IAM)** lehetőséget a bal oldalon, és válassza a **Hozzáadás** lehetőséget az oldal tetején.

A legördülő Szerepkör listában válassza a **Számlakezelő** lehetőséget. Adja meg a felhasználó e-mail-címét a hozzáférés megadásához. Válassza a **Mentés** lehetőséget a szerepkör hozzárendeléséhez.
