---
title: Értekezlet-házirend beállításai
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: dac06690b51459ca166c15a5ef0f4c7e7a6d36f0
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376676"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Értekezletházirendek kezelése a Microsoft teamben

Az értekezletre vonatkozó házirendek a szervezet felhasználói által ütemezett értekezletekhez rendelkezésre álló szolgáltatások vezérlésének ellenőrzésére szolgálnak. Az értekezletre vonatkozó házirendek egyes funkciói még nem valósulhatnak meg a csapatok admin központban (ezeket a dokumentációban "hamarosan" felirattal kell címkézni). Ebben az esetben, vagy ha Ön szerzés egy hiba szeret "mi vidám ' korszerűsíteni a politika éppen most de megpróbál ez újra később"-ban Mikroszkóp fuvaros admin központ, mi ajánl amit ön használ PowerShell-hoz teremt vagy módosít fuvaros találkozó politikák. 

A következő forrásokból tájékozódhat az értekezletre vonatkozó házirendekkel kapcsolatban:

- A házirendek létrehozásával, a módosításokkal és a felhasználóknak a házirendhez való hozzárendelésével kapcsolatos tudnivalókat [az értekezletházirendek kezelése a csapatokban](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams)című témakörben talál.

- A házirendek módosításának PowerShell-parancsmagokkal való használatához lásd a [csapatok PowerShell – áttekintés](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)című témakört. 
    - Meg kell használni a [Skype for Business PowerShell modult](https://www.microsoft.com/download/details.aspx?id=39366) az olyan csapatoknak, amelyek a házirendeket tárgyalnak. 
    - A további tudnivalókért tanulmányozza a [*-csteamsmeetingpolicy parancsmagok dokumentációját](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) .

**Megjegyzés:** A házirend-módosítások érvénybe léptetéséhez akár 24 óráig is eltarthat. Előfordulhat, hogy azonnal nem tudja módosítani az újonnan létrehozott házirendeket; várjon 4 órát, majd próbálja meg újra módosítani az újonnan létrehozott házirendet. Ha-a ' csendes birtoklás probléma, megpróbál PowerShell.  