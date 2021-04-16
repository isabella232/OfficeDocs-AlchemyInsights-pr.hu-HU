---
title: Titkosítás átviteli szabályokkal
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: dfd77bc83b4b278e3630858f54fdfb109ade2a14
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813870"
---
# <a name="encryption-with-transport-rules"></a>Titkosítás átviteli szabályokkal

Az [Exchange Felügyeleti központban](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) az e-mail-forgalom szabályain belül az Office üzenettitkosítási (OME) lehetőségeket használhatja az üzenettitkosítás elindítására. Az Átviteli szabály feltételén válassza az **Office 365 Üzenettitkosítás és a tartalomvédelem alkalmazása** lehetőséget.

- További információ: [Az e-mail-forgalom szabályainak meghatározása a titkosításhoz](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- A PowerShellben használja a [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) parancsmagot, és állítsa az *ApplyOME* paramétert $true értékre.
