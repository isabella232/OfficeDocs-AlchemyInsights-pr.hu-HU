---
title: Hibakód 0x15
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
description: Ha hibaüzenet jelenik meg az Office 2013 távoli asztali szolgáltatások (RDS) telepítésekor, fontolja meg az ADAL engedélyezését a beállításjegyzék szerkesztésével.
ms.openlocfilehash: 247686bf26c11d07ed118bdb1ba190fc718e87cf140b88f79b8aa0b40c827b4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54100764"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Hiba a 2013-as Office távoli asztali szolgáltatások aktiválása során

Ha hibaüzenet jelenik meg az Office 2013 távoli asztali szolgáltatások (RDS) telepítésekor, fontolja meg az ADAL engedélyezését a beállításjegyzék szerkesztésével.
  
|**Beállításkulcs**|**Típus**|**Érték**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

További információ: A modern hitelesítés engedélyezése Office [2013](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)esetén Windows eszközökön.
  
> [!NOTE]
>  Az ADAL alapértelmezés szerint engedélyezve van a 2016-Nagyvállalati Microsoft 365-alkalmazások és Office-ban. A Távoli asztali szolgáltatások neve korábban Terminálszolgáltatások volt.
  