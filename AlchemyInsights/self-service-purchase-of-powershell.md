---
title: A PowerShell önkiszolgáló vásárlása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3516"
ms.openlocfilehash: e6cc504ebef19cbe78f576d9b207fe2d951d0ef5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47739972"
---
# <a name="self-service-purchase-of-powershell"></a>A PowerShell önkiszolgáló vásárlása

A MSCommerce PowerShell-modul használatához telepítenie kell azt Windows 10-es eszközön a TLS 1,2 (szükséges helyi rendszergazdai engedélyekkel).  Importálás és csatlakozás a MSCommerce modulhoz.  Amikor a rendszer arra kéri, hogy jelentkezzen be, globális vagy számlázási rendszergazdai szerepkör-hitelesítő adatokat kell használnia.  

Ha nincs TLS 1,2, a következő hibaüzenet jelenhet meg a házirend beszerzése vagy frissítése során:

*ErrorMessage – az alapul szolgáló kapcsolat bezárult: váratlan hiba történt a küldésben*.



