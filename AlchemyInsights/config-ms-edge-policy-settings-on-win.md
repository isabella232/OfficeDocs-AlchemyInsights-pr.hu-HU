---
title: A Microsoft Edge házirend-beállításainak megadása a Windowsban
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
- "6894"
ms.openlocfilehash: 7f626152c3833638436dfe05e8dcd13fc86ef594
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583443"
---
# <a name="configure-microsoft-edge-policy-settings-on-windows"></a><span data-ttu-id="6bc25-102">A Microsoft Edge házirend-beállításainak megadása a Windowsban</span><span class="sxs-lookup"><span data-stu-id="6bc25-102">Configure Microsoft Edge policy settings on Windows</span></span>

<span data-ttu-id="6bc25-103">Ha konfigurálni szeretné a házirend-beállításokat és a Microsoft Edge felügyelt frissítéseit, használja a csoportházirend-objektumokat (GPO-k).</span><span class="sxs-lookup"><span data-stu-id="6bc25-103">To configure policy settings and managed updates for Microsoft Edge, use Group Policy Objects (GPOs).</span></span> <span data-ttu-id="6bc25-104">A házirendet a beállításjegyzéken keresztül is megadhatja; Ez a megfelelő (1) Windows-eszközök Microsoft Active Directory-tartományhoz, illetve (2) Windows 10-es Pro-és nagyvállalati verzióhoz csatlakoztak, amelyek az eszközkezelés Microsoft Intune-ben lettek bejelentkezve.</span><span class="sxs-lookup"><span data-stu-id="6bc25-104">You can also provision policy through the registry; this would be appropriate for (1) Windows devices joined to a Microsoft Active Directory domain and for (2) Windows 10 Pro and Enterprise instances enrolled for device management in Microsoft Intune.</span></span>

<span data-ttu-id="6bc25-105">Ha a Microsoft Edge-et csoportházirend-objektumokkal szeretné konfigurálni, tegye az alábbiakat:</span><span class="sxs-lookup"><span data-stu-id="6bc25-105">To configure Microsoft Edge by using GPOs, do the following:</span></span>

1. <span data-ttu-id="6bc25-106">Ha az Active Directory-tartományban a csoportházirend központi tárolója vagy az egyes számítógépeken a házirend-definíciós sablon mappája van, telepítse a Microsoft Edge szabályait és beállításait tartalmazó összes felügyeleti sablont.</span><span class="sxs-lookup"><span data-stu-id="6bc25-106">To the Group Policy Central Store in your Active Directory domain, or to the Policy Definition template folder on individual computers, install all administrative templates that add rules and settings for Microsoft Edge.</span></span>
2. <span data-ttu-id="6bc25-107">Állítsa be a beállítani kívánt házirendeket.</span><span class="sxs-lookup"><span data-stu-id="6bc25-107">Configure the specific policies you want to set.</span></span>

<span data-ttu-id="6bc25-108">További információt [a Microsoft Edge-házirend beállításainak megadása a Windowsban](https://go.microsoft.com/fwlink/?linkid=2135024)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="6bc25-108">To learn more, see [Configure Microsoft Edge policy settings on Windows](https://go.microsoft.com/fwlink/?linkid=2135024).</span></span>
