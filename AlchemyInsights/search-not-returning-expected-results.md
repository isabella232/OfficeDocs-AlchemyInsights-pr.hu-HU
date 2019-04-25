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
ms.custom: 1491
ms.assetid: ''
ms.openlocfilehash: 517d9b75fc3aef09c0c2d5870aa695cc0ab10f06
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32383837"
---
# <a name="content-search-not-returning-expected-results"></a>Tartalom keresés nem a várt eredmények visszaadása

Tartalom keresése az Office 365 biztonsági & Megfelelési központba történő futtatásakor váratlan keresési eredményeket kaphat. Vegye figyelembe, amelyek hatással lehetnek a keresési eredmények a következők:

- **Tartalom helye és a keresési feltételek**: Ellenőrizze, hogy a megfelelő tartalom helyének kiválasztott keresési feltételek. Ha futtatta a nagy keresés (a számos helyen), érdemes több megkeresi azokat a darabolás.

- **Részben indexelt elem**: a becsült keresési eredmények [részben indexelt elem](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) a postafiókok szerepelnek. Azonban a OneDrive és a SharePoint-webhelyekről történő részleges indexelt elem nem szerepelnek a keresési becslés.

- **Sikertelen keresés**: nagyszámú postafiókot (több mint 100 000 postafiókok) keresésekor jelenhet meg keresési hibák, a hibakódok CS008-009 és CS012-002). Ebben az esetben próbálja meg újra a keresés csak a sikertelen tartalom helye. [Ez a cikk](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) további információt talál.
