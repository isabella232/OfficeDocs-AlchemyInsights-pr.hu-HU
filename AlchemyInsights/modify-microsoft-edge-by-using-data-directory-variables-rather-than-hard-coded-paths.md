---
title: A Microsoft Edge módosítása kódolt elérési utak helyett adatkönyvtár-változók használatával
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8222"
- "9004596"
ms.openlocfilehash: 23ce69157c465c56d0fc5ada7c2c159e3192fd75
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035819"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a>A Microsoft Edge módosítása kódolt elérési utak helyett adatkönyvtár-változók használatával

Ha például a Windowsban a profiladatokat egy felhasználó helyi alkalmazásadatai között, nem pedig az alapértelmezett helyen tárolja, állítsa a *UserDataDir házirendet* **${local_app_data}\Edge\Profile** helyre.

További információ: [Felhasználói Microsoft Edge-adattárak változóinak létrehozása.](https://docs.microsoft.com/deployedge/microsoft-edge-policies)