---
title: A tartalomvédelmi szolgáltatás konfigurációjának tesztelése az új OME-funkciókhoz
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12428"
- "9000078"
ms.openlocfilehash: 62697d6379ea6ab3c6af86d3bab752af560da7c1250e5ef6dd2a3eae8023a05e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812437"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>A tartalomvédelmi szolgáltatás konfigurációjának tesztelése az új OME-funkciókhoz

Ha ellenőrizni, hogy a Microsoft 365 konfigurálva van-e az új OME-funkciók használatára, futtassa az alábbi parancsmagokat, miközben csatlakozik Exchange Online [PowerShellhez:](/powershell/exchange/exchange-online-powershell)


1. Ellenőrizze a bérlő tartalomvédelmi konfigurációját a következő `Get-IRMConfiguration` futtatásával: . Győződjön meg arról, hogy ezek az értékek True **(Igaz) értéket tartalmaznak:**
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. A tartományt, a feladó címét és a címzettet használva futtassa a `Test-IRMConfiguration` () et. Ha a teszt nem működik, vizsgálja meg a tartalomvédelmi szolgáltatás konfigurációját.

A tartalomvédelmi szolgáltatás konfigurációjának ellenőrzéséhez az Új OME-konfiguráció ellenőrzése a [PowerShellben Exchange Online információt.](/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell)