---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 2c4d8e075d2cf7214b5ef005b856daf7fb0ed53c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710445"
---
# <a name="verify-your-domain"></a><span data-ttu-id="778a0-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="778a0-102">Verify your domain</span></span>

 <span data-ttu-id="778a0-103">**A bejegyzés valószínűleg nem frissült az interneten.**</span><span class="sxs-lookup"><span data-stu-id="778a0-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="778a0-104">Általában csak néhány percet vesz igénybe, hogy láthassuk az új rekordot, de néha akár néhány órát is igénybe vehet.</span><span class="sxs-lookup"><span data-stu-id="778a0-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="778a0-105">Ha már ilyen régóta várt, ellenőrizze, hogy a pontos értéket másolta-e és illesztette-e be a DNS-szolgáltató TXT-ellenőrzési rekordjába.</span><span class="sxs-lookup"><span data-stu-id="778a0-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="778a0-106">Az egyik gyakori probléma, hogy nem tartalmazza a rekord "MS=" részét.</span><span class="sxs-lookup"><span data-stu-id="778a0-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="778a0-107">Arra is szükségünk van!</span><span class="sxs-lookup"><span data-stu-id="778a0-107">We need that too!</span></span>

- <span data-ttu-id="778a0-108">Egyes DNS-állomásokon további lépést kell tennie a zónafájl (ahol a DNS-rekord tárolása) mentéséhez szükséges, hogy az az interneten keresztül frissüljön.</span><span class="sxs-lookup"><span data-stu-id="778a0-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="778a0-109">Győződjön meg arról, hogy mentette a módosításokat, hogy a Microsoft láthassa és ellenőrizhesse a bejegyzést.</span><span class="sxs-lookup"><span data-stu-id="778a0-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
