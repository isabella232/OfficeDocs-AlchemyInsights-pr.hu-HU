---
title: Tartomány névkiszolgálóinak frissítése, hogy a Microsoftra irányuljanak
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: d9d66e366db14840a86b681deba78b89ddff5e068a3b931c88e493d2ec791b10
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54073602"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a>Tartomány névkiszolgálóinak frissítése, hogy a Microsoftra irányuljanak

Megjegyzés: A névkiszolgáló-módosítások elterjedéséhez néha 48 órára is szükség lehet.
  
Ahhoz, hogy beállítsa a tartományát a Microsoftnál, frissítenie kell a tartományregisztráló névkiszolgálóit. Hozza létre vagy szerkessze a névkiszolgálói rekordokat a tartományregisztrálójánál.
  
1. Nyissa meg a tartományregisztrálója webhelyét, és keresse meg a névkiszolgálók szerkesztésére szolgáló területet.

2. Hozzon létre vagy szerkesszen két névkiszolgálói rekordot úgy, hogy a következő értékeket tartalmazzák:

  - ns1.bdm.microsoftonline.com

  - ns2.bdm.microsoftonline.com

3. Mentse a módosításokat.

Részletes útmutatást ebben a cikkben is talál: A névkiszolgálók módosítása úgy, hogy Microsoft 365 [tartományregisztrálónál beállítsa a rekordokat.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)
  