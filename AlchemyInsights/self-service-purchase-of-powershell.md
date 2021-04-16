---
title: A PowerShell önkiszolgáló megvásárlása
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3516"
ms.openlocfilehash: 48b5b0a1be1bc03d45a531a1093f18a3f750c37d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51797723"
---
# <a name="self-service-purchase-of-powershell"></a>A PowerShell önkiszolgáló megvásárlása

Az MSCommerce PowerShell modult TLS 1.2-es TLS 1.2-es Windows 10-es eszközre kell telepítenie (helyi rendszergazdai engedélyek szükségesek).  Importálja az MSCommerce modult, és csatlakozzon ahhoz.  Amikor a rendszer arra kéri, hogy jelentkezzen be, a globális vagy számlázási rendszergazdai szerepkörhöz szükséges hitelesítő adatokat kell használnia.  

Ha nem TLS 1.2-es, a következő hibaüzenet jelenhet meg, amikor megkísérli be szerezni vagy frissíteni a házirendet:

*ErrorMessage – A mögöttes kapcsolat lezárult: Váratlan* hiba történt egy küldésen.



