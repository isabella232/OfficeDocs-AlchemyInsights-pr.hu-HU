---
title: 'Hiba: A számítógépen nem egyeznek meg a szabályok'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782954"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="a5197-102">Hiba: A számítógépen nem egyeznek meg a szabályok</span><span class="sxs-lookup"><span data-stu-id="a5197-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="a5197-103">Az ismert probléma frissített állapotának megtekintése: A számítógépen nem egyeznek meg a [Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0) szabályai</span><span class="sxs-lookup"><span data-stu-id="a5197-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="a5197-104">Az Outlook csapata végrehajtott egy javítást a 12928.10000-es buildben.</span><span class="sxs-lookup"><span data-stu-id="a5197-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="a5197-105">A javítás már az Insider Fast szinten van, és 2020. június végén a Havi csatornán is létezik.</span><span class="sxs-lookup"><span data-stu-id="a5197-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="a5197-106">Miután a javított buildet javította, még egyszer megkérdezheti, hogy melyik szabályokat szeretné megtartani.</span><span class="sxs-lookup"><span data-stu-id="a5197-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="a5197-107">Amikor a rendszer kéri, válassza a Kiszolgáló lehetőséget, majd menjen vissza az Outlookba, és engedélyezze újra a letiltott szabályokat.</span><span class="sxs-lookup"><span data-stu-id="a5197-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="a5197-108">A javítás elérhetővé válik, kérjük, használja az alábbi kerülő megoldást:</span><span class="sxs-lookup"><span data-stu-id="a5197-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="a5197-109">**Kerülő** megoldás: A legutóbbi jelentések szerint a probléma olyan ügyfeleknél fordult elő, akik csak az Outlook asztali verziójában hoztak létre ügyféloldali szabályokat.</span><span class="sxs-lookup"><span data-stu-id="a5197-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="a5197-110">Ha a probléma továbbra is fennáll, érdemes törölni a szabályokat, majd csak az Outlook Web Appban létrehozni és szerkeszteni a szabályokat, amíg a probléma meg nem oldódik.</span><span class="sxs-lookup"><span data-stu-id="a5197-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="a5197-111">Ha nem tudja manuálisan törölni a szabályokat, futtathat egy Outlook-parancsot az Outlook elindítani a /cleanrules Outlook.exe futtatásával.</span><span class="sxs-lookup"><span data-stu-id="a5197-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="a5197-112">Ezzel az ügyfél és a kiszolgáló szabályait is törli.</span><span class="sxs-lookup"><span data-stu-id="a5197-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="a5197-113">Ezzel törli az Outlook-profilban az összes fiók összes szabályát.</span><span class="sxs-lookup"><span data-stu-id="a5197-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="a5197-114">Ezt a parancsot a Parancssori kapcsolók cikkben is olvashatja.</span><span class="sxs-lookup"><span data-stu-id="a5197-114">This command is further documented in the Command-line switches article.</span></span>

