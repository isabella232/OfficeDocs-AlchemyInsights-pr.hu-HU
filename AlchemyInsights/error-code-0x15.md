---
title: 0x15-ös hibakód
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Ha az Office 2013 távoli asztali szolgáltatások (RDS) telepítéseken való aktiválásakor hibaüzenetet kap, a beállításjegyzék szerkesztésével engedélyezheti az ADAL szolgáltatást.
ms.openlocfilehash: 566d63cbe37d295b3546b9d7d5b14dfc8e8fe0ec
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703140"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="60d09-103">Hiba az Office 2013 aktiválása közben a Távoli asztali szolgáltatásokszolgáltatásban</span><span class="sxs-lookup"><span data-stu-id="60d09-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="60d09-104">Ha az Office 2013 távoli asztali szolgáltatások (RDS) telepítéseken való aktiválásakor hibaüzenetet kap, a beállításjegyzék szerkesztésével engedélyezheti az ADAL szolgáltatást.</span><span class="sxs-lookup"><span data-stu-id="60d09-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="60d09-105">**Beállításkulcs**</span><span class="sxs-lookup"><span data-stu-id="60d09-105">**Registry key**</span></span>|<span data-ttu-id="60d09-106">**Típus**</span><span class="sxs-lookup"><span data-stu-id="60d09-106">**Type**</span></span>|<span data-ttu-id="60d09-107">**Érték**</span><span class="sxs-lookup"><span data-stu-id="60d09-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="60d09-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="60d09-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="60d09-109">Reg_dword</span><span class="sxs-lookup"><span data-stu-id="60d09-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="60d09-110">1</span><span class="sxs-lookup"><span data-stu-id="60d09-110">1</span></span>  <br/> |

<span data-ttu-id="60d09-111">További információt az [Office 2013 modern hitelesítésének engedélyezése Windows-eszközökön című témakörben talál.](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)</span><span class="sxs-lookup"><span data-stu-id="60d09-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="60d09-112">Az ADAL alapértelmezés szerint engedélyezve van a Nagyvállalati Microsoft 365 alkalmazásokban és az Office 2016-ban.</span><span class="sxs-lookup"><span data-stu-id="60d09-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="60d09-113">A Távoli asztali szolgáltatások (RDS) neve korábban Terminálszolgáltatások volt.</span><span class="sxs-lookup"><span data-stu-id="60d09-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  