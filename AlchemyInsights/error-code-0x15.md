---
title: 'Hibakód: 0x15'
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Ha Office 2013 aktiválása a távoli asztali szolgáltatások (RDS) telepítések közben hibaüzenetet kap, érdemes megfontolni a ADAL a rendszerleíró adatbázis szerkesztésével.
ms.openlocfilehash: e2249d8ebbd2313c64dda5656a3243fa76d97a9a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35388247"
---
<span data-ttu-id="401b5-103">Ha Office 2013 aktiválása a távoli asztali szolgáltatások (RDS) telepítések közben hibaüzenetet kap, érdemes megfontolni a ADAL a rendszerleíró adatbázis szerkesztésével.</span><span class="sxs-lookup"><span data-stu-id="401b5-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="401b5-104">**Beállításkulcs**</span><span class="sxs-lookup"><span data-stu-id="401b5-104">**Registry key**</span></span>|<span data-ttu-id="401b5-105">**Típus**</span><span class="sxs-lookup"><span data-stu-id="401b5-105">**Type**</span></span>|<span data-ttu-id="401b5-106">**Érték**</span><span class="sxs-lookup"><span data-stu-id="401b5-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="401b5-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="401b5-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="401b5-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="401b5-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="401b5-109">1</span><span class="sxs-lookup"><span data-stu-id="401b5-109">1</span></span>  <br/> |

<span data-ttu-id="401b5-110">További tudnivalókért tanulmányozza a [Windows eszközök Office 2013 Modern hitelesítés engedélyezése](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="401b5-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="401b5-111">ADAL Office 365 ProPlus és Office 2016 alapértelmezés szerint engedélyezve van.</span><span class="sxs-lookup"><span data-stu-id="401b5-111">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="401b5-112">Távoli asztali szolgáltatások (RDS) > korábban a Terminálszolgáltatások neve volt.</span><span class="sxs-lookup"><span data-stu-id="401b5-112">>  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  