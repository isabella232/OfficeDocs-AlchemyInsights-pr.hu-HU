---
title: Megoldódott a nyomtatásisor-kezelő hibája
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
ms.openlocfilehash: 66b39434ef6f9ad2b8392f811704e67c1bcffd2b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801843"
---
# <a name="print-spooler-issue-is-resolved"></a>Megoldódott a nyomtatásisor-kezelő hibája

Ha az eszközét a Windows 10  **OS 19041,329-es verzióval**frissítette, lehet, hogy megfigyelte azt a hibát, amely miatt egyes nyomtatók nem nyomtathatók ki. A nyomtatásisor-kezelő hibát okozhat, vagy váratlanul bezárul, amikor megpróbál kinyomtatni, és a kimenet nem érkezik meg az érintett nyomtatóból. Ezt a hibát a 19041,331-es verzió ( **19041.331**-es összeállítás) [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).  

**Folyamatban lévő vizsgálat**

Előfordulhat, hogy az LSASS-fájl (**Isass.exe**) néhány eszközön sikertelen lesz, és a hibaüzenet "a kritikus rendszerfolyamat, C:\WINDOWS\system32\Isass.exe, sikertelen volt az állapotkód c0000008. A gépet most újra kell indítani.  **A Microsoft a megoldáson dolgoznak, és egy későbbi kiadásban frissítést fog biztosítani.**

További információért olvassa el a  [Windows 10 2004-es verzió ismert problémái](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc)című témakört.