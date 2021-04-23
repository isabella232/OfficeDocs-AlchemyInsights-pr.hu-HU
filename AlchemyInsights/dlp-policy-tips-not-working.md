---
title: Nem működnek a DLP-házirendtippek
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 8a3b8175c077b77d1c9b5d859012faddcb1fa3a0
ms.sourcegitcommit: 099704f7f4bdf122d09bb4f7cc71d36fc77a7fcf
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2021
ms.locfileid: "51958704"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="c2fe6-102">DLP-házirend tippekkel kapcsolatos problémák</span><span class="sxs-lookup"><span data-stu-id="c2fe6-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="c2fe6-103">**Fontos**: Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive szolgáltatások továbbra is mindig hozzáférhetők legyenek – További információt a [SharePoint Online Ideiglenes funkciómódosítások](https://aka.ms/ODSPAdjustments) oldalon olvashat.</span><span class="sxs-lookup"><span data-stu-id="c2fe6-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="c2fe6-104">Ha házirendtippeket konfigurálni a DLP-házirendhez a Biztonsági & megfelelőségi központban teljes kényszerítési módban, tegye a következőket:</span><span class="sxs-lookup"><span data-stu-id="c2fe6-104">To configure policy tips on your DLP policy in the Security & Compliance center in full enforcement mode, do the following:</span></span>

- <span data-ttu-id="c2fe6-105">Győződjön meg arról, hogy engedélyezve vannak **a** házirendtippek a DLP-szabályon.</span><span class="sxs-lookup"><span data-stu-id="c2fe6-105">Ensure policy tips have been **enabled** on the DLP rule.</span></span> <span data-ttu-id="c2fe6-106">A lépéseket az [E-mail-értesítések küldése és a DLP-házirendekkel kapcsolatos házirendtippek megjelenítése.](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="c2fe6-106">For steps, see [Send email notifications and show policy tips for DLP policies](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="c2fe6-107">Győződjön meg arról, hogy a tartalom megfelel a Bizalmas adattípusú entitások definícióiban ismertetett szabály [alkalmazásához szükséges feltételeknek.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="c2fe6-107">Ensure your content matches what is required to trigger the rule outlined in [Sensitive information type entity definitions](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="c2fe6-108">A házirendtippek az Outlook Web Appban és az Outlookban egyaránt megjelennek.</span><span class="sxs-lookup"><span data-stu-id="c2fe6-108">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="c2fe6-109">Az Outlook 2013-as vagy újabb verziójában azonban csak bizonyos feltételek mellett jelennek meg a házirendtippek.</span><span class="sxs-lookup"><span data-stu-id="c2fe6-109">However, when using Outlook 2013 or later, policy tips are displayed only under certain conditions.</span></span> <span data-ttu-id="c2fe6-110">A konkrét feltételek listáját Az Outlook 2013-as vagy újabb verziójának támogatott feltételei című témakörben [olvashatja el a házirendtippek megjelenítéséhez.](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="c2fe6-110">For the specific conditions list, see [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span></span>

<span data-ttu-id="c2fe6-111">A DLP-házirendtippekkel [](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps) kapcsolatos információkért lásd: DLP-házirendtippek – tippek és támogatási mátrixok a [DLP-házirendtippek használatához.](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps)</span><span class="sxs-lookup"><span data-stu-id="c2fe6-111">For information on DLP Policy tips, see [DLP Policy Tips Reference](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps) and [Support Matrix for DLP Policy tips](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps).</span></span>