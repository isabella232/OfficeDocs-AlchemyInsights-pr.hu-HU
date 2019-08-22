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
ms.openlocfilehash: 4ef2943e5a529368fa2c614e4431cf180924fbb8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527002"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="2e81b-103">Hiba történt a távoli asztali szolgáltatások Office 2013 aktiválás</span><span class="sxs-lookup"><span data-stu-id="2e81b-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="2e81b-104">Ha Office 2013 aktiválása a távoli asztali szolgáltatások (RDS) telepítések közben hibaüzenetet kap, érdemes megfontolni a ADAL a rendszerleíró adatbázis szerkesztésével.</span><span class="sxs-lookup"><span data-stu-id="2e81b-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="2e81b-105">**Beállításkulcs**</span><span class="sxs-lookup"><span data-stu-id="2e81b-105">**Registry key**</span></span>|<span data-ttu-id="2e81b-106">**Típus**</span><span class="sxs-lookup"><span data-stu-id="2e81b-106">**Type**</span></span>|<span data-ttu-id="2e81b-107">**Érték**</span><span class="sxs-lookup"><span data-stu-id="2e81b-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="2e81b-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="2e81b-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="2e81b-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="2e81b-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="2e81b-110">1</span><span class="sxs-lookup"><span data-stu-id="2e81b-110">1</span></span>  <br/> |

<span data-ttu-id="2e81b-111">További tudnivalókért tanulmányozza a [Windows eszközök Office 2013 Modern hitelesítés engedélyezése](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="2e81b-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="2e81b-112">ADAL Office 365 ProPlus és Office 2016 alapértelmezés szerint engedélyezve van.</span><span class="sxs-lookup"><span data-stu-id="2e81b-112">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="2e81b-113">Távoli asztali szolgáltatások (RDS) korábban a Terminálszolgáltatások neve volt.</span><span class="sxs-lookup"><span data-stu-id="2e81b-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  