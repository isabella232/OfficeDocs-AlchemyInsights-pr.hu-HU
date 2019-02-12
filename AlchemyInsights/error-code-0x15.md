---
title: 'Hibakód: 0x15'
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Ha Office 2013 aktiválása a távoli asztali szolgáltatások (RDS) telepítések közben hibaüzenetet kap, érdemes megfontolni a ADAL a rendszerleíró adatbázis szerkesztésével.
ms.openlocfilehash: 6d4076ecb5c6ee3c3cf4c4610ad4aa29ab477d8a
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29929090"
---
<span data-ttu-id="c9925-103">Ha Office 2013 aktiválása a távoli asztali szolgáltatások (RDS) telepítések közben hibaüzenetet kap, érdemes megfontolni a ADAL a rendszerleíró adatbázis szerkesztésével.</span><span class="sxs-lookup"><span data-stu-id="c9925-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="c9925-104">**Beállításkulcs**</span><span class="sxs-lookup"><span data-stu-id="c9925-104">**Registry key**</span></span>|<span data-ttu-id="c9925-105">**Típus**</span><span class="sxs-lookup"><span data-stu-id="c9925-105">**Type**</span></span>|<span data-ttu-id="c9925-106">**Érték**</span><span class="sxs-lookup"><span data-stu-id="c9925-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="c9925-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="c9925-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="c9925-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="c9925-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="c9925-109">1</span><span class="sxs-lookup"><span data-stu-id="c9925-109">1</span></span>  <br/> |
   
<span data-ttu-id="c9925-110">További tudnivalókért tanulmányozza a [Windows eszközök Office 2013 Modern hitelesítés engedélyezése](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="c9925-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="c9925-p101">ADAL Office 365 ProPlus és Office 2016 alapértelmezés szerint engedélyezve van. Távoli asztali szolgáltatások (RDS) > korábban a Terminálszolgáltatások neve volt.</span><span class="sxs-lookup"><span data-stu-id="c9925-p101">ADAL is enabled by default in Office 365 ProPlus and Office 2016. >  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

