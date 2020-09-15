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
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Hiba az Office 2013 távoli asztali szolgáltatásokban való aktiválásakor

Ha hibaüzenet jelenik meg, miközben az Office 2013-t a Remote Desktop Services (RDS) környezetben aktiválja, érdemes lehet a ADAL a beállításjegyzék szerkesztésével engedélyezni.
  
|**Beállításkulcs**|**Típus**|**Érték**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

További információt [a modern hitelesítés engedélyezése az Office 2013 Windows rendszerű eszközökön](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)című témakörben talál.
  
> [!NOTE]
>  A ADAL alapértelmezés szerint engedélyezve van a Microsoft 365 Enterprise és az Office 2016 rendszerhez. A Remote Desktop Services (RDS) korábban "Terminal Services" néven lett elnevezve.
  