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
ms.openlocfilehash: a187fec34ef3eae485a8a880127b5f82a028edb7f0e9a276a41b5e33cad25ead
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53942837"
---
# <a name="self-service-purchase-of-powershell"></a>A PowerShell önkiszolgáló megvásárlása

Az MSCommerce PowerShell modult TLS 1.2-es Windows 10 rendelkező Windows 10 kell telepítenie (helyi rendszergazdai engedélyek szükségesek).  Importálja az MSCommerce modult, és csatlakozzon ahhoz.  Amikor a rendszer arra kéri, hogy jelentkezzen be, a globális vagy számlázási rendszergazdai szerepkörhöz szükséges hitelesítő adatokat kell használnia.  

Ha nem TLS 1.2-es, a következő hibaüzenet jelenhet meg, amikor megkísérli be szerezni vagy frissíteni a házirendet:

*ErrorMessage – A mögöttes kapcsolat lezárult: Váratlan* hiba történt egy küldésen.



