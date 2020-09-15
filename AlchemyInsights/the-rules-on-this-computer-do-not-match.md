---
title: 'Hiba: a számítógépen lévő szabályok nem egyeznek meg'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c2feb6da651d8b3eb7af6a057335b28d26f9e7f6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690965"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="6e330-102">Hiba: a számítógépen lévő szabályok nem egyeznek meg</span><span class="sxs-lookup"><span data-stu-id="6e330-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="6e330-103">Ha az ismert probléma frissített állapotát szeretné látni, tanulmányozza [a számítógépen lévő szabályok nem egyeznek meg a Microsoft Exchange szabályaival](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="6e330-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="6e330-104">Az Outlook csapata végrehajtotta a 12928,10000-es verzió javítását.</span><span class="sxs-lookup"><span data-stu-id="6e330-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="6e330-105">A javítás már az Insider Fast-on van, és a havi csatorna 2020 június végén fog kinézni.</span><span class="sxs-lookup"><span data-stu-id="6e330-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="6e330-106">Miután megadta a fix összeállítást, a következő üzenet jelenik meg: "milyen szabályok szerint szeretné megőrizni az időt".</span><span class="sxs-lookup"><span data-stu-id="6e330-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="6e330-107">Válassza a kiszolgáló lehetőséget, amikor a rendszer kéri, majd térjen vissza az Outlookba, és engedélyezze újra a letiltott szabályokat.</span><span class="sxs-lookup"><span data-stu-id="6e330-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="6e330-108">Amíg a javítás elérhetővé nem válik, kérjük, használja az alábbi kerülő megoldást:</span><span class="sxs-lookup"><span data-stu-id="6e330-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="6e330-109">**Kerülő megoldás**: a legutóbbi jelentésekben a probléma abban az esetben fordult elő, ha az asztali Outlookban csak az ügyfél-szabályokat hozta létre.</span><span class="sxs-lookup"><span data-stu-id="6e330-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="6e330-110">Ha továbbra is fennáll a probléma, fontolja meg a szabályok törlését, majd csak az OWA (Outlook Web App) alkalmazásban hozzon létre és szerkesszen szabályokat a probléma megoldásához.</span><span class="sxs-lookup"><span data-stu-id="6e330-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="6e330-111">Ha nem tudja törölni a szabályokat manuálisan, akkor futtathatja az Outlook parancsát, ha a Outlook.exe/cleanrules. futtatja az Outlookot.</span><span class="sxs-lookup"><span data-stu-id="6e330-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="6e330-112">Ez az ügyfél-és kiszolgálói szabályok törlését is törli.</span><span class="sxs-lookup"><span data-stu-id="6e330-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="6e330-113">Törli az Outlook-profil összes fiókjának összes szabályát.</span><span class="sxs-lookup"><span data-stu-id="6e330-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="6e330-114">Ezt a parancsot részletesebben a parancssori kapcsolók című cikk ismerteti.</span><span class="sxs-lookup"><span data-stu-id="6e330-114">This command is further documented in the Command-line switches article.</span></span>

