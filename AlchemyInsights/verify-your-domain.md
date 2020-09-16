---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: d30f9b51c0164acd126f214a581ad6cec5eec04e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734308"
---
# <a name="verify-your-domain"></a><span data-ttu-id="78afe-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="78afe-102">Verify your domain</span></span>

 <span data-ttu-id="78afe-103">**A rekord valószínűleg nem frissült az interneten keresztül.**</span><span class="sxs-lookup"><span data-stu-id="78afe-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="78afe-104">Ez általában csak néhány percet vesz igénybe, hogy megtekintse az új rekordot, de alkalmanként csak néhány órát vehet igénybe.</span><span class="sxs-lookup"><span data-stu-id="78afe-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="78afe-105">Ha már várta, hogy már régóta, ellenőrizze, hogy másolta-e a pontos értéket a DNS-szolgáltatójánál a TXT-ellenőrző rekordba.</span><span class="sxs-lookup"><span data-stu-id="78afe-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="78afe-106">Egy gyakori probléma nem tartalmazza a rekord "MS =" részét.</span><span class="sxs-lookup"><span data-stu-id="78afe-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="78afe-107">Ehhez is szükségünk van!</span><span class="sxs-lookup"><span data-stu-id="78afe-107">We need that too!</span></span>

- <span data-ttu-id="78afe-108">Bizonyos DNS-szolgáltatóknak további lépésekkel kell elvégezniük a zónafájl mentését (ahol a DNS-rekord tárolva van), hogy a fájl az interneten keresztül frissüljön.</span><span class="sxs-lookup"><span data-stu-id="78afe-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="78afe-109">Ellenőrizze, hogy mentette-e a módosításokat, így a Microsoft láthatja és ellenőrizheti a rekordot.</span><span class="sxs-lookup"><span data-stu-id="78afe-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
