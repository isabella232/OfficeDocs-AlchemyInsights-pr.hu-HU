---
title: Előfordulhat, hogy a DLP-nek egyéni típusra van szüksége
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: c0996e0cc923c13b7de3752ac6534026e8627c51
ms.sourcegitcommit: dcd1c76ced1a0cec27f4cf8d383593760c198424
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/18/2021
ms.locfileid: "59446693"
---
# <a name="dlp-might-need-a-custom-type"></a>Előfordulhat, hogy a DLP-nek egyéni típusra van szüksége

**Fontos**: Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive szolgáltatások továbbra is mindig hozzáférhetők legyenek – További információt a [SharePoint Online Ideiglenes funkciómódosítások](https://aka.ms/ODSPAdjustments) oldalon olvashat.

**A DLP egyéni adattípust is megkövetelhet**

Az adatveszteség-megelőzési (DLP)-házirendekkel azonosíthatja és megvédheti a bizalmas adatokat a szervezetében. Bizonyos esetekben előfordulhat, hogy létre kell hoznia egy saját bizalmasadat-típust a szervezet adatainak védelméhez. További információt a Bizalmas adattípusok [és](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-learn-about) [a Bizalmas adattípusú entitásdefiníciók megismerése.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

Az egyéni bizalmas adattípusok és házirendek létrehozásáról további információt az itt található: 

**Beépített bizalmas adattípus testreszabása**

Ha egy beépített bizalmas adattípus csupán néhány finomítással megfelelne az igényeinek, tekintse meg a Beépített bizalmas adattípus [testreszabása tájékoztatást.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type) Felvehet vagy eltávolíthat például kulcsszavakat, illetve hozzáadhat vagy eltávolíthat támogató bizonyítékokat, például dátumot vagy címet.

**Egyéni bizalmas adattípus létrehozása**

Ha azonban különböző típusú bizalmas információkat kell azonosítania és védenie, létrehozhat egy egyéni bizalmas adattípust a Microsoft 365 Megfelelőségi központ. További információt az Egyéni bizalmas adattípusok – első [lépések.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type)

**Egyéni bizalmas információtípus létrehozása a Biztonsági & PowerShellben**

Végül, ha a felhasználói felület nem biztosít minden szükséges lehetőséget, létrehozhat egy egyéni bizalmas adattípust a Biztonsági & PowerShellben. Xml-fájllal kezdődően az összes elérhető beállítást használhatja. További információ: Egyéni bizalmas adattípus [létrehozása a PowerShell használatával.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell)

Ha először tesztmódban tesztelné [](https://docs.microsoft.com/microsoft-365/compliance/dlp-learn-about-dlp#implement-policy-in-test-mode) a házirendet, tekintse meg a Házirend implementálja tesztelési módban és [a DLP-házirend létrehozása,](https://docs.microsoft.com/microsoft-365/compliance/create-test-tune-dlp-policy)tesztelése és finomhangolása a következőt: . 