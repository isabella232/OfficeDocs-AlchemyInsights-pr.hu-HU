---
title: 'Hibakód: 0x15'
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Ha Office 2013 aktiválása a távoli asztali szolgáltatások (RDS) telepítések közben hibaüzenetet kap, érdemes megfontolni a ADAL a rendszerleíró adatbázis szerkesztésével.
ms.openlocfilehash: 89f9270169e13fd7706f7826c624ef8ae4d47b3f
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28293667"
---
<span data-ttu-id="fe4f8-103">Ha Office 2013 aktiválása a távoli asztali szolgáltatások (RDS) telepítések közben hibaüzenetet kap, érdemes megfontolni a ADAL a rendszerleíró adatbázis szerkesztésével.</span><span class="sxs-lookup"><span data-stu-id="fe4f8-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="fe4f8-104">**Beállításkulcs**</span><span class="sxs-lookup"><span data-stu-id="fe4f8-104">**Registry key**</span></span>|<span data-ttu-id="fe4f8-105">**Típus**</span><span class="sxs-lookup"><span data-stu-id="fe4f8-105">**Type**</span></span>|<span data-ttu-id="fe4f8-106">**Érték**</span><span class="sxs-lookup"><span data-stu-id="fe4f8-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="fe4f8-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="fe4f8-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="fe4f8-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="fe4f8-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="fe4f8-109">1</span><span class="sxs-lookup"><span data-stu-id="fe4f8-109">1</span></span>  <br/> |
   
<span data-ttu-id="fe4f8-110">További tudnivalókért tanulmányozza a [Windows eszközök Office 2013 Modern hitelesítés engedélyezése](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="fe4f8-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="fe4f8-p101">ADAL Office 365 ProPlus és Office 2016 alapértelmezés szerint engedélyezve van. > A távoli asztali szolgáltatások (RDS) korábban a Terminálszolgáltatások neve volt.</span><span class="sxs-lookup"><span data-stu-id="fe4f8-p101">ADAL is enabled by default in Office 365 ProPlus and Office 2016. >  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

