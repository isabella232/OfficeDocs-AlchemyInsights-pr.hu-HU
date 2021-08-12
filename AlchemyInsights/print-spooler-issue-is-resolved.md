---
title: Megoldottuk a nyomtatásisor-kezelővel kapcsolatban problémát.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 73ff86928c043dd41f49d456d30c2fcf7947bd4cb304d0456c634d4fa5808239
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911340"
---
# <a name="print-spooler-issue-is-resolved"></a>Megoldottuk a nyomtatásisor-kezelővel kapcsolatban problémát.

Ha az eszközt az Windows 10 **19041.329-es** buildjére frissítettük, előfordulhat, hogy bizonyos nyomtatók nem nyomtatnak.   A nyomtatási várólista hibát okozhat, vagy váratlanul bezárulhat nyomtatás közben, és az érintett nyomtató nem hoz létre kimenetet. Ezt a problémát az operációs rendszer **19041.331-es** és [KB4567523-as buildjában megoldottuk.](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523)  

**Folyamatban lévő vizsgálat**

Előfordulhat, hogy a helyi biztonsági alrendszerszolgáltatás (LSASS) fájlja (**Isass.exe**) egyes eszközökön sikertelen lehet a "Kritikus rendszer-folyamat, C:\WINDOWS\system32\Isass.exe, nem sikerült a c0000008 állapotkóddal. A gépet most újra kell indítani".  **A Microsoft dolgozik a megoldáson, és egy közelgő kiadásban frissíteni fog.**

További információt a [2004-es Windows 10](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc)ismert problémáiról ad.