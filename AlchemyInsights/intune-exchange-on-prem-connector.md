---
title: Intune-alapú Exchange helyi összekötő
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 8b470655efa2dfb460c29b6b840fa793ed2aa448
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807647"
---
# <a name="intune-exchange-on-premise-connector"></a>Intune-alapú Exchange helyi összekötő

A helyszíni Intune és az Exchange közötti kapcsolat beállításáról az alábbi dokumentációban tájékozódhat:

[Az Intune helyszíni Exchange-összekötő beállítása a Microsoft Intune Azure-ban](https://docs.microsoft.com/intune/exchange-connector-install)

**GYAKORI kérdések**

K: egy hibaüzenet jelenik meg, például "az Exchange Connector verziója nem támogatott" hibaüzenet jelenik meg az Exchange-összekötő beállításakor. Mi lehet az oka?

A: a használt fiók megfelelő licenccel rendelkezik – aktív Intune licenccel kell rendelkeznie.

K: lehet több Exchange összekötőt is?

A: csak egyetlen Exchange-csatlakozót állíthat be egy Intune-bérlői fiókhoz egy Exchange-szervezetben. Az összekötő csak egy kiszolgálón telepíthető több kiszolgálós Exchange-szervezetben.

Az egyazon bérlői fiókban konfigurált Exchange-és Exchange Online-kapcsolatokhoz is nincs konfigurálva az összekötők.

K: használhatók-e az összekötők CAS-tömbökkel az Exchange-kapcsolaton keresztül?

A: a CAS-tömb megadása nem támogatott konfiguráció az összekötő beállításai között. Csak egyetlen kiszolgálót kell megadni, és az összekötő konfigurációs fájlban kell hardcoded, amely megtalálható

program data\microsoft\microsoft Intune a helyi Exchange-csatlakozón \ OnpremiseExchangeConnectorServiceConfiguration.xml

Keresse meg a következő bejegyzést ```<ExchangeWebServiceURL />``` , és cserélje le az URL-t az Exchange-kiszolgálóval.

**Például**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

További hibaelhárítási információkat az alábbi dokumentációban talál: [Intune helyszíni Exchange-összekötő hibaelhárítása](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Az Exchange összekötő részletes naplózásának engedélyezése**

1. Nyissa meg szerkesztésre az Exchange Connector-nyomkövetési konfigurációs fájlt.  
A fájl a következő helyen található:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Például**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Keresse meg a TraceSourceLine a következő kulccsal: OnPremisesExchangeConnectorService  
  
3. A SourceLevel csomópont értékének módosítása az adatok ActivityTracing (az alapértelmezett) a bőbeszédű ActivityTracing  

**Például**
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. A Microsoft Intune Exchange szolgáltatás újraindítása  
5. Teljes szinkronizálás az Intune-portálon, amíg el nem fejeződik, majd az XML visszaváltása "információs ActivityTracing", majd indítsa újra a Microsoft Intune Exchange szolgáltatást.  
6. A naplók helye: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`