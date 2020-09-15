---
title: 0x15 hibakód
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Ha hibaüzenet jelenik meg, miközben az Office 2013-t a Remote Desktop Services (RDS) környezetben aktiválja, érdemes lehet a ADAL a beállításjegyzék szerkesztésével engedélyezni.
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709189"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="4c807-103">Hiba az Office 2013 távoli asztali szolgáltatásokban való aktiválásakor</span><span class="sxs-lookup"><span data-stu-id="4c807-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="4c807-104">Ha hibaüzenet jelenik meg, miközben az Office 2013-t a Remote Desktop Services (RDS) környezetben aktiválja, érdemes lehet a ADAL a beállításjegyzék szerkesztésével engedélyezni.</span><span class="sxs-lookup"><span data-stu-id="4c807-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="4c807-105">**Beállításkulcs**</span><span class="sxs-lookup"><span data-stu-id="4c807-105">**Registry key**</span></span>|<span data-ttu-id="4c807-106">**Típus**</span><span class="sxs-lookup"><span data-stu-id="4c807-106">**Type**</span></span>|<span data-ttu-id="4c807-107">**Érték**</span><span class="sxs-lookup"><span data-stu-id="4c807-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="4c807-108">HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="4c807-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="4c807-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="4c807-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="4c807-110">1</span><span class="sxs-lookup"><span data-stu-id="4c807-110">1</span></span>  <br/> |

<span data-ttu-id="4c807-111">További információt [a modern hitelesítés engedélyezése az Office 2013 Windows rendszerű eszközökön](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="4c807-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="4c807-112">A ADAL alapértelmezés szerint engedélyezve van a Microsoft 365 Enterprise és az Office 2016 rendszerhez.</span><span class="sxs-lookup"><span data-stu-id="4c807-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="4c807-113">A Remote Desktop Services (RDS) korábban "Terminal Services" néven lett elnevezve.</span><span class="sxs-lookup"><span data-stu-id="4c807-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  