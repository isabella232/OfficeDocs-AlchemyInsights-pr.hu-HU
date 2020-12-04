---
title: Meghatalmazott hozzáadása vagy eltávolítása a Windows Outlookban
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573580"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a>Meghatalmazott hozzáadása vagy eltávolítása a Windows Outlookban

Meghatalmazott felvétele a Windows Outlookban: 

1. Kattintson a **fájl** fülre, majd a **Fiókbeállítások** elemre, és válassza a **meghatalmazotti hozzáférés** parancsot.
2. Kattintson a **Hozzáadás** gombra. Ha a **Hozzáadás** nem jelenik meg, lehetséges, hogy az Outlook és az Exchange között nem létezik aktív kapcsolat. Az Outlook állapotsora megjeleníti a kapcsolat állapotát.
3. Írja be a meghatalmazottként kijelölni kívánt személy nevét, vagy keresse meg és jelölje ki a nevet a keresési eredmények listájában.

    > [!NOTE]
    > A meghatalmazottnak a szervezet Exchange-alapú globális címjegyzékében (GAL) kell lennie.
4. Kattintson a **Hozzáadás** elemre, majd **az OK gombra**.
5. A **meghatalmazott engedélyei** párbeszédpanelen fogadja el az alapértelmezett jogosultsági beállításokat, vagy válassza az egyéni hozzáférési szintek lehetőséget az Exchange-mappákhoz.

    - Ha a meghatalmazottnak engedélyt kell adni csak az értekezlet-összehívásokkal és a válaszokkal való munkára, az alapértelmezett engedélyezési beállítások (például a meghatalmazott) az **értekezlettel kapcsolatos üzenetek másolatait kapják meg** . A **Beérkezett üzenetekre** vonatkozó engedélyt a **none** értékre hagyhatja. Az értekezlet-összehívások és válaszok közvetlenül a meghatalmazott postaládájába kerülnek.

    > [!NOTE]
    > Alapértelmezés szerint a meghatalmazott **szerkesztő (elemek olvasása, létrehozása és módosítása)** engedélye van a **Naptár** mappájához. Amikor a meghatalmazott az Ön nevében válaszol az értekezletre, a program automatikusan hozzáadja a **Naptár** mappához.

5. Ha üzenetet szeretne küldeni a meghatalmazottnak a módosított engedélyekről, jelölje be az **üzenet automatikus küldése a meghatalmazottnak az engedélyek összegzése** jelölőnégyzetet.
6. Tetszés szerint jelölje be a **meghatalmazott láthatja a magánjellegű elemeket** jelölőnégyzetet.

    > [!IMPORTANT]
    > Ez a beállítás az összes Exchange-mappára hatással van. Ide tartozik a minden levél, a névjegyek, a naptár, a feladatok, a feljegyzések és a Journal-mappák. Csak a megadott mappákban lévő magánjellegű elemekhez lehet hozzáférést adni.

7. Kattintson az **OK** gombra.

    > [!NOTE]
    >
    > - A Küldés más nevében engedélyekkel küldött üzeneteket a meghatalmazott és a **Feladó** neve melletti nevek is magukban foglalják. Ha egy üzenetet küldés másként engedéllyel küld el, csak a neve jelenik meg.
    > - Miután felvesz valakit meghatalmazottként, felveheti az Exchange-postaládáját az Outlook-profiljába. Útmutatásért olvassa el a [másik személy leveleinek és naptárának kezelése című cikket](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).

Meghatalmazott eltávolítása a Windows Outlookban:

1. Kattintson a **fájl** fülre.
2. Kattintson a **Fiókbeállítások** elemre, majd a **meghatalmazotti hozzáférés** elemre.
3. Jelölje ki annak a meghatalmazottnak a nevét, akinek meg szeretné változtatni az engedélyeit, majd kattintson az **Eltávolítás** után **az OK gombra**.
