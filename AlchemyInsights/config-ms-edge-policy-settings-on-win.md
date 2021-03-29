---
title: A Microsoft Edge házirendbeállításainak konfigurálása Windows rendszeren
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003845"
- "9004632"
- "6894"
- "8358"
ms.openlocfilehash: e9bb489b4d8ecd76fd777ade9fb740ecad542900
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402377"
---
# <a name="configure-microsoft-edge-policy-settings-on-windows"></a><span data-ttu-id="d6dd8-102">A Microsoft Edge házirendbeállításainak konfigurálása Windows rendszeren</span><span class="sxs-lookup"><span data-stu-id="d6dd8-102">Configure Microsoft Edge policy settings on Windows</span></span>

<span data-ttu-id="d6dd8-103">A Microsoft Edge házirendbeállításai és felügyelt frissítései a Csoportházirend-objektumok (GPOS) segítségével konfigurálhatóak.</span><span class="sxs-lookup"><span data-stu-id="d6dd8-103">To configure policy settings and managed updates for Microsoft Edge, use Group Policy Objects (GPOs).</span></span> <span data-ttu-id="d6dd8-104">A házirendeket a beállításjegyzéken keresztül is kiépítheti; ez a (1) Microsoft Active Directory tartományhoz csatlakozott Windows-eszközök és (2) a Microsoft Intune-ban eszközkezelésre regisztrált Windows 10 Pro és Enterprise példány esetén lenne megfelelő.</span><span class="sxs-lookup"><span data-stu-id="d6dd8-104">You can also provision policy through the registry; this would be appropriate for (1) Windows devices joined to a Microsoft Active Directory domain and for (2) Windows 10 Pro and Enterprise instances enrolled for device management in Microsoft Intune.</span></span>

<span data-ttu-id="d6dd8-105">Ha a Microsoft Edge-et GPOs-okkal konfigurálni, tegye a következőket:</span><span class="sxs-lookup"><span data-stu-id="d6dd8-105">To configure Microsoft Edge by using GPOs, do the following:</span></span>

1. <span data-ttu-id="d6dd8-106">Az Active Directory-tartomány csoportházirendek – központi tárolója vagy az egyes számítógépeken a Policy Definition (Házirend-definíció) sablonmappába telepítve telepítse az összes olyan felügyeleti sablont, amely a Microsoft Edge-hez szabályokat és beállításokat ad hozzá.</span><span class="sxs-lookup"><span data-stu-id="d6dd8-106">Go to the Group Policy Central Store in your Active Directory domain, or to the Policy Definition template folder on individual computers, install all administrative templates that add rules and settings for Microsoft Edge.</span></span>
2. <span data-ttu-id="d6dd8-107">Konfigurálja a beállítani kívánt házirendeket.</span><span class="sxs-lookup"><span data-stu-id="d6dd8-107">Configure the specific policies you want to set.</span></span>

<span data-ttu-id="d6dd8-108">További információ: [A Microsoft Edge házirendbeállításainak konfigurálása Windows rendszeren.](https://go.microsoft.com/fwlink/?linkid=2135024)</span><span class="sxs-lookup"><span data-stu-id="d6dd8-108">To learn more, see [Configure Microsoft Edge policy settings on Windows](https://go.microsoft.com/fwlink/?linkid=2135024).</span></span>
