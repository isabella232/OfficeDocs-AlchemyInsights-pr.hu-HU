---
title: Titkosítás átviteli szabályokkal
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: 3f16c7e7be99a50cd57f47ea2801b3022c4aec95
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915177"
---
# <a name="encryption-with-transport-rules"></a>Titkosítás átviteli szabályokkal

Az [Exchange Felügyeleti központban](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) az e-mail-forgalom szabályain belül az Office üzenettitkosítási (OME) lehetőségeket használhatja az üzenettitkosítás elindítására. Az Átviteli szabály feltételén válassza az **Office 365 Üzenettitkosítás és a tartalomvédelem alkalmazása** lehetőséget.

- További információ: [Az e-mail-forgalom szabályainak meghatározása a titkosításhoz](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- A PowerShellben használja a [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) parancsmagot, és állítsa az *ApplyOME* paramétert $true értékre.
