---
title: Előfordulhat, hogy a DLP-nek egyéni típusra van szüksége
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932660"
---
# <a name="dlp-might-need-a-custom-type"></a>Előfordulhat, hogy a DLP-nek egyéni típusra van szüksége

**Fontos:** Sok SharePoint Online- és OneDrive-ügyfél üzleti szempontból kritikus fontosságú alkalmazásokat futtat a háttérben futó szolgáltatással szemben. Ezek közé tartozik a tartalomáttelepítés, az adatveszteség-megelőzés (DLP) és a biztonsági mentési megoldások. Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive-szolgáltatások magas rendelkezésre állásúak és megbízhatóak maradjanak a távoli munkahelyi helyzetekben minden eddiginél jobban függő felhasználók számára.

Ennek a célkitűzésnek a támogatása érdekében szigorúbb szabályozási korlátokat vezettünk be a háttéralkalmazásokra (áttelepítés, DLP és biztonsági mentési megoldások) a hétköznapokon. Meg kell várni, hogy ezek az alkalmazások elérése nagyon korlátozott átviteli ezekben az időkben. Azonban a régió esti és hétvégi óráiban a szolgáltatás készen áll arra, hogy jelentősen nagyobb mennyiségű kérést dolgozzon fel a háttéralkalmazásokból.

**A DLP-hez egyéni információtípusra lehet szükség**

Az adatvesztés-megelőzési (DLP) házirenddel azonosíthatja és megvédheti a szervezeten belüli bizalmas adatokat. Bizonyos esetekben előfordulhat, hogy létre kell hoznia saját **egyéni** bizalmas információtípusát a szervezet adatainak védelme érdekében.

Előfordulhat például, hogy a szervezetnek azonosítania és védenie kell az alkalmazottazonosítókat vagy más adatokat a szervezetre jellemző formátumban. Ha igen, további információt az alábbi cikkekben talál.
  
 **Beépített bizalmas információtípus testreszabása**
  
Ha egy beépített bizalmas információtípus néhány csípéssel megfelel az igényeinek, [testreszabhatja a beépített bizalmas információtípust.](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type) Hozzáadhat vagy eltávolíthat például kulcsszavakat, illetve hozzáadhat vagy eltávolíthat alátámasztó bizonyítékokat, például dátumot vagy címet.
  
 **Egyéni bizalmas információtípus létrehozása**
  
Ha azonban egy másik típusú bizalmas információt kell azonosítania és védenie, [létrehozhat egy egyéni bizalmas információtípust](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) a Biztonsági & megfelelőségi központ felhasználói felületén.
  
**Egyéni bizalmas információtípus létrehozása a Security & Compliance Center PowerShell ben**

Végül, ha a felhasználói felület nem biztosítja az összes szükséges beállítást, [létrehozhat egy egyéni bizalmas információtípust a Security & Compliance Center PowerShell ben.](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell) Az XML-fájllal kezdve minden elérhető lehetőséget használhat.
