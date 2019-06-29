---
title: 1491-Search-not-returning-Expected-Results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d25c1ef2e0e746432472a436cb11d25b5db5596c
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35355879"
---
# <a name="content-search-not-returning-expected-results"></a>Tartalom keresés nem a várt eredmények visszaadása

Tartalom keresése az Office 365 biztonsági & Megfelelési központba történő futtatásakor váratlan keresési eredményeket kaphat. Vegye figyelembe, amelyek hatással lehetnek a keresési eredmények a következők:

- **Tartalom helye és a keresési feltételek**: Ellenőrizze, hogy a megfelelő tartalom helyének kiválasztott keresési feltételek. Ha futtatta a nagy keresés (a számos helyen), érdemes több megkeresi azokat a darabolás.

- **Részben indexelt elem**: a becsült keresési eredmények [részben indexelt elem](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) a postafiókok szerepelnek. Azonban a OneDrive és a SharePoint-webhelyekről történő részleges indexelt elem nem szerepelnek a keresési becslés.

- **Sikertelen keresés**: nagyszámú postafiókot (több mint 100 000 postafiókok) keresésekor jelenhet meg keresési hibák, a hibakódok CS008-009 és CS012-002). Ebben az esetben próbálja meg újra a keresés csak a sikertelen tartalom helye. [Ez a cikk](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) további információt talál.
