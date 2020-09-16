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
ms.openlocfilehash: 7322fa640f6d043f057c8b7a5e06a18dcd10eec5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734913"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a>Tartomány névkiszolgálóinak frissítése, hogy a Microsoftra irányuljanak

Megjegyzés: A névkiszolgáló-módosítások elterjedéséhez néha 48 órára is szükség lehet.
  
A tartománynak a Microsofttal való beállításához frissíteni kell a tartományregisztrálónál a névkiszolgálói szolgáltatókat. Hozza létre vagy szerkessze a névkiszolgálói rekordokat a tartományregisztrálójánál.
  
1. Nyissa meg a tartományregisztrálója webhelyét, és keresse meg a névkiszolgálók szerkesztésére szolgáló területet.

2. Hozzon létre vagy szerkesszen két névkiszolgálói rekordot úgy, hogy a következő értékeket tartalmazzák:

  - ns1.bdm.microsoftonline.com

  - ns2.bdm.microsoftonline.com

3. Mentse a módosításokat.

Ebben a cikkben részletes útmutatást talál: a [Névkiszolgálók módosítása a Microsoft 365 bármely tartományregisztrálónál való beállításához](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)
  