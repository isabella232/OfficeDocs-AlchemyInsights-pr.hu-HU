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
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="b70aa-102">Megoldódott a nyomtatásisor-kezelő hibája</span><span class="sxs-lookup"><span data-stu-id="b70aa-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="b70aa-103">Ha az eszközét a Windows 10  **OS 19041,329-es verzióval**frissítette, lehet, hogy megfigyelte azt a hibát, amely miatt egyes nyomtatók nem nyomtathatók ki.</span><span class="sxs-lookup"><span data-stu-id="b70aa-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="b70aa-104">A nyomtatásisor-kezelő hibát okozhat, vagy váratlanul bezárul, amikor megpróbál kinyomtatni, és a kimenet nem érkezik meg az érintett nyomtatóból.</span><span class="sxs-lookup"><span data-stu-id="b70aa-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="b70aa-105">Ezt a hibát a 19041,331-es verzió ( **19041.331**-es összeállítás) [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span><span class="sxs-lookup"><span data-stu-id="b70aa-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="b70aa-106">**Folyamatban lévő vizsgálat**</span><span class="sxs-lookup"><span data-stu-id="b70aa-106">**Ongoing investigation**</span></span>

<span data-ttu-id="b70aa-107">Előfordulhat, hogy az LSASS-fájl (**Isass.exe**) néhány eszközön sikertelen lesz, és a hibaüzenet "a kritikus rendszerfolyamat, C:\WINDOWS\system32\Isass.exe, sikertelen volt az állapotkód c0000008.</span><span class="sxs-lookup"><span data-stu-id="b70aa-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="b70aa-108">A gépet most újra kell indítani.</span><span class="sxs-lookup"><span data-stu-id="b70aa-108">The machine must now be restarted".</span></span>  <span data-ttu-id="b70aa-109">**A Microsoft a megoldáson dolgoznak, és egy későbbi kiadásban frissítést fog biztosítani.**</span><span class="sxs-lookup"><span data-stu-id="b70aa-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="b70aa-110">További információért olvassa el a  [Windows 10 2004-es verzió ismert problémái](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc)című témakört.</span><span class="sxs-lookup"><span data-stu-id="b70aa-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>