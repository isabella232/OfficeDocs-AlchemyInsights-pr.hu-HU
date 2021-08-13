---
title: Az SharePoint korlátozása klasszikus módra
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 6315a83ac825f96ceea60798d441de8e8e53336fe29eda4d0491dd8a6a43b352
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53958803"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>Az SharePoint korlátozása klasszikus módra

Egyes szervezeteknek továbbra is szükségük van a klasszikus módra. Bár nem tervezi a klasszikus mód részletes eltávolítását, a listák és tárak esetében a továbbiakban nem lehet a teljes szervezet (bérlő) klasszikus módjára korlátozni.

A rendszergazdának az alábbi lehetőségei vannak az egyes listák és tárak klasszikus módban való kezelésére a részletes, az alábbi szinteken elérhető leiratkozási kapcsolók használatával:

- webhelycsoport
- webhely
- lista
- tár

Ezenkívül a bizonyos funkciókat és testreszabásokat nem támogató, a modern verzió által nem támogatott listákat a rendszer továbbra is klasszikus módra váltja.

2019. április 1-től kezdődően meg fog kezdődni és folytatódik a modern listák és tárak bérlői szintű letiltási folyamata 2019. május 31-ig.  A bérlő letiltásából eredő klasszikus módban található listák és tárak automatikusan modernre váltódnak.

Ha klasszikus módot igényel, [](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) itt további információkat és [](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) A PnP Powershell használatát ismertetve megtudhatja, hogy milyen lehetőségeket és eszközöket használhat a klasszikus mód használatában.
