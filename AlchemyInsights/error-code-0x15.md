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
ms.openlocfilehash: 468d13e59602cf173ed2e17af44c66babfc28703
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506848"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Hiba az Office 2013 aktiválása közben a Távoli asztali szolgáltatásokszolgáltatásban

Ha az Office 2013 távoli asztali szolgáltatások (RDS) telepítéseken való aktiválásakor hibaüzenetet kap, a beállításjegyzék szerkesztésével engedélyezheti az ADAL szolgáltatást.
  
|**Beállításkulcs**|**Típus**|**Érték**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

További információt az [Office 2013 modern hitelesítésének engedélyezése Windows-eszközökön című témakörben talál.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)
  
> [!NOTE]
>  Az ADAL alapértelmezés szerint engedélyezve van a Nagyvállalati Microsoft 365 alkalmazásokban és az Office 2016-ban. A Távoli asztali szolgáltatások (RDS) neve korábban Terminálszolgáltatások volt.
  