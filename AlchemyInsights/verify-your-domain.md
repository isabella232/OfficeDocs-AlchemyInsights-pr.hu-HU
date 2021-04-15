---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 4a34de7fa2aaaae365cf4562d31590d4b5fb7544
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51770993"
---
# <a name="verify-your-domain"></a><span data-ttu-id="066bc-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="066bc-102">Verify your domain</span></span>

 <span data-ttu-id="066bc-103">**A rekord valószínűleg nem frissült az interneten keresztül.**</span><span class="sxs-lookup"><span data-stu-id="066bc-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="066bc-104">Az új rekordot általában csak néhány percig tart, de időnként akár néhány óráig is eltarthat.</span><span class="sxs-lookup"><span data-stu-id="066bc-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="066bc-105">Ha ilyen sokáig várt, ellenőrizze, hogy pontosan a PONTOS értéket másolta-e be a DNS-szolgáltatóNÁL található TXT rekordba.</span><span class="sxs-lookup"><span data-stu-id="066bc-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="066bc-106">Gyakori probléma, hogy a rekord nem tartalmazza az "MS=" részt.</span><span class="sxs-lookup"><span data-stu-id="066bc-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="066bc-107">Arra is szükség van!</span><span class="sxs-lookup"><span data-stu-id="066bc-107">We need that too!</span></span>

- <span data-ttu-id="066bc-108">Egyes DNS-szolgáltatónál további lépéssel mentenie kell a zónafájlt (ahol a DNS-rekordot tárolja), hogy az szerte az interneten frissülni fog.</span><span class="sxs-lookup"><span data-stu-id="066bc-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="066bc-109">Győződjön meg arról, hogy mentette a módosításokat, hogy a Microsoft lássa és ellenőrizni tudja a rekordot.</span><span class="sxs-lookup"><span data-stu-id="066bc-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
