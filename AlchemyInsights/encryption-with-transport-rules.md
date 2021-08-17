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
ms.openlocfilehash: e1f8227047daede71d0fa3b3557db0d95a379b99b76ab0c2fe1d6ed8cc213d4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079452"
---
# <a name="encryption-with-transport-rules"></a>Titkosítás átviteli szabályokkal

Az [Exchange Felügyeleti központban](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) az e-mail-forgalom szabályain belül az Office üzenettitkosítási (OME) lehetőségeket használhatja az üzenettitkosítás elindítására. Az Átviteli szabály feltételén válassza az **Office 365 Üzenettitkosítás és a tartalomvédelem alkalmazása** lehetőséget.

- További információ: [Az e-mail-forgalom szabályainak meghatározása a titkosításhoz](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- A PowerShellben használja a [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) parancsmagot, és állítsa az *ApplyOME* paramétert $true értékre.
