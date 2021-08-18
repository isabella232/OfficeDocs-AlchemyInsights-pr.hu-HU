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
ms.openlocfilehash: ed3770c001461c162ff5bbe24dc400a29380a03b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316688"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Hiba a 2013-as Office távoli asztali szolgáltatások aktiválása során

Ha hibaüzenet jelenik meg az Office 2013 távoli asztali szolgáltatások (RDS) telepítésekor, fontolja meg az ADAL engedélyezését a beállításjegyzék szerkesztésével.
  
|**Beállításkulcs**|**Típus**|**Érték**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

További információ: A modern hitelesítés engedélyezése Office [2013-ban Windows eszközökön.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)
  
**Megjegyzés:** Az ADAL alapértelmezés szerint engedélyezve van a 2016-os Nagyvállalati Microsoft 365-alkalmazások és Office-ben. A Távoli asztali szolgáltatások neve korábban Terminálszolgáltatások volt.
  