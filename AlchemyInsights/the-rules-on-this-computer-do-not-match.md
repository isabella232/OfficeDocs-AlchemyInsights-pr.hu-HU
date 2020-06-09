---
title: 'Hiba: A számítógépen lévő szabályok nem egyeznek'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c0982da82826d1644f437b19e0d343a59d7ac473
ms.sourcegitcommit: e09af4285c6b81ca0a5320fdb811713ac25748c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/09/2020
ms.locfileid: "44664248"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="f6844-102">Hiba: A számítógépen lévő szabályok nem egyeznek</span><span class="sxs-lookup"><span data-stu-id="f6844-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="f6844-103">Az ismert probléma frissített állapotának megtekintéséhez olvassa el [A számítógépen lévő szabályok nem egyeznek meg a Microsoft Exchange szabályaival.](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="f6844-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="f6844-104">Az Outlook Csapat megvalósított egy javítást az 12928.10000 buildben.</span><span class="sxs-lookup"><span data-stu-id="f6844-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="f6844-105">A javítás már az Insider Fast-nál van, és 2020 júniusának végén a Monthly Channel-re kerül.</span><span class="sxs-lookup"><span data-stu-id="f6844-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="f6844-106">Miután a fix épít lehet, hogy a gyors "Milyen szabályokat akarsz tartani" még egyszer utoljára.</span><span class="sxs-lookup"><span data-stu-id="f6844-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="f6844-107">Ha a rendszer kéri, válassza a Kiszolgáló lehetőséget, majd lépjen vissza az Outlook programban, és engedélyezze újra a letiltott szabályokat.</span><span class="sxs-lookup"><span data-stu-id="f6844-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="f6844-108">Amíg a javítás elérhetővé nem válik, használja a következő kerülő megoldást:</span><span class="sxs-lookup"><span data-stu-id="f6844-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="f6844-109">**Megoldás:** A legutóbbi jelentésekben a probléma azok esetében fordult elő, akik csak ügyfélszabályokat hoztak létre az Outlook asztalon.</span><span class="sxs-lookup"><span data-stu-id="f6844-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="f6844-110">Ha továbbra is problémákkal küzd, fontolja meg a szabályok törlését, majd csak az OWA (Outlook Web App) alkalmazásban hozzon létre és szerkesztsen szabályokat, amíg a probléma meg nem oldódik.</span><span class="sxs-lookup"><span data-stu-id="f6844-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="f6844-111">Ha nem tudja manuálisan törölni a szabályokat, az Outlook program indításakor az Outlook/cleanrules paranccsal is futtathatja az Outlook parancsát.</span><span class="sxs-lookup"><span data-stu-id="f6844-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="f6844-112">Ezzel az ügyfél- és a kiszolgálói szabályt is törli.</span><span class="sxs-lookup"><span data-stu-id="f6844-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="f6844-113">Törli az Outlook-profil összes fiókjának összes szabályát.</span><span class="sxs-lookup"><span data-stu-id="f6844-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="f6844-114">Ezt a parancsot a Parancssori kapcsolók cikk tovább dokumentálja.</span><span class="sxs-lookup"><span data-stu-id="f6844-114">This command is further documented in the Command-line switches article.</span></span>

