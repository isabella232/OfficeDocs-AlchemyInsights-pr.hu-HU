---
title: Intune Exchange-összekötő
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
ms.openlocfilehash: 744758739c2ca839823d2c8b440ed7b0d9dd4f06ebbb6f19fe52041a6710c4b4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013966"
---
# <a name="intune-exchange-on-premise-connector"></a>Intune Exchange-összekötő

Az Intune és a helyszínen üzemeltetett összekötő Exchange az alábbi dokumentációban olvashat részletesen:

[Az Intune helyszíni összekötő Exchange beállítása Microsoft Intune Azure-ban](https://docs.microsoft.com/intune/exchange-connector-install)

**Gyakori kérdések:**

K: A "The Exchange Connector version is not supported" (A Exchange Connector verziója nem támogatott) hibaüzenet jelenik meg, amikor megkísérli beállítani a Exchange összekötőt. Mi lehet az oka?

A: A használt fiók licence a megfelelő – aktív Intune-licenccel kell

K: Több összekötő is Exchange lehet?

A: Intune-bérlőnként csak egy összekötőt Exchange szervezetenként Exchange beállítani. Az összekötő csak egy kiszolgálóra telepíthető egy többkiszolgálós exchange-szervezetben.

Ezenkívül nem konfigurálhat összekötőket mind a Exchange, mind a Exchange Online konfigurálva ugyanabban a bérlői fiókban.

K: Az összekötő használható CAS-tömböt a Exchange?

A: A CAS-tömb megadása nem támogatott konfiguráció az összekötő beállításában. Csak egyetlen kiszolgálót kell megadni, és az összekötő konfigurációs fájljában kell megadni, amely megtalálható a

program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml

Keresse meg az alábbi bejegyzést, ```<ExchangeWebServiceURL />``` és cserélje le az URL-címet az Exchange-kiszolgálóra.

**Példa:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

További hibaelhárításért olvassa el az alábbi dokumentációt: Az Intune helyszíni hibaelhárítása Exchange [összekötővel](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Verbose naplózás engedélyezése a Exchange összekötőhöz**

1. Nyissa meg Exchange összekötő nyomkövetési konfigurációs fájlját szerkesztésre.  
A fájl a következő helyen található: %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Példa:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Keresse meg a TraceSourceLine-t a következő kulccsal: OnPremisesExchangeConnectorService  
  
3. A SourceLevel csomópont értékének módosítása Information ActivityTracing (alapértelmezett) értékről Verbose ActivityTracing értékre  

**Példa:**
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
4. A Microsoft Intune Exchange újraindítása  
5. Teljes szinkronizálás az Intune Portalon, amíg be nem fejezi, majd az XML-t "Információs tevékenységsáv" formátumúra módosítja, és újraindítja a Microsoft Intune Exchange szolgáltatást.  
6. A naplók helye: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`