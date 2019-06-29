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
Ha Office 2013 aktiválása a távoli asztali szolgáltatások (RDS) telepítések közben hibaüzenetet kap, érdemes megfontolni a ADAL a rendszerleíró adatbázis szerkesztésével.
  
|**Beállításkulcs**|**Típus**|**Érték**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

További tudnivalókért tanulmányozza a [Windows eszközök Office 2013 Modern hitelesítés engedélyezése](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL Office 365 ProPlus és Office 2016 alapértelmezés szerint engedélyezve van. Távoli asztali szolgáltatások (RDS) > korábban a Terminálszolgáltatások neve volt.
  