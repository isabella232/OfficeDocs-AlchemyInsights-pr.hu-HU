---
title: 1490-hibaelhárítás-eDiscovery-hibák
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277833"
---
# <a name="troubleshoot-content-search-errors"></a>Tartalmi keresési hibák elhárítása

Problémákat tapasztal a tartalmi kereséssel kapcsolatban, vagy problémákat tapasztal a keresési eredmények exportálásakor?

A keresések futtatásakor például a következőket kapja meg?

- CS008 vagy CS012 hibák

- A kiszolgáló foglalt/időtúllépési hibája

- Alkalmazási hiba történt

Vagy ha nagy számú postaládából keres vagy exportál találatokat (több mint 100 000-postaládában), az exportálási hibákat kapja?

Az ilyen típusú hibák esetén próbálkozzon a sikertelenül megjelenő tartalmi helyek keresésével. További információt  [ebben a cikkben](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) talál.

Ha több, mint 100K postaládát exportál, a következő PowerShell-lel kell használnia az Exportálás eredményének letöltéséhez:  [eredmények exportálása több mint 100k postaládából](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).
