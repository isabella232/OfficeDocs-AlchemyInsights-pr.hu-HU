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
ms.openlocfilehash: 4df8c49880fe638c1659f76edc0905532d091e45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820828"
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
