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
# <a name="intune-exchange-on-premise-connector"></a><span data-ttu-id="f5be3-102">Intune-alapú Exchange helyi összekötő</span><span class="sxs-lookup"><span data-stu-id="f5be3-102">Intune Exchange on-premise Connector</span></span>

<span data-ttu-id="f5be3-103">A helyszíni Intune és az Exchange közötti kapcsolat beállításáról az alábbi dokumentációban tájékozódhat:</span><span class="sxs-lookup"><span data-stu-id="f5be3-103">For details of setting up the connector between Intune and Exchange which is hosted on-premises please see the following documentation:</span></span>

[<span data-ttu-id="f5be3-104">Az Intune helyszíni Exchange-összekötő beállítása a Microsoft Intune Azure-ban</span><span class="sxs-lookup"><span data-stu-id="f5be3-104">Set up the Intune on-premises Exchange connector in Microsoft Intune Azure</span></span>](https://docs.microsoft.com/intune/exchange-connector-install)

<span data-ttu-id="f5be3-105">**GYAKORI kérdések**</span><span class="sxs-lookup"><span data-stu-id="f5be3-105">**FAQ:**</span></span>

<span data-ttu-id="f5be3-106">K: egy hibaüzenet jelenik meg, például "az Exchange Connector verziója nem támogatott" hibaüzenet jelenik meg az Exchange-összekötő beállításakor.</span><span class="sxs-lookup"><span data-stu-id="f5be3-106">Q: I see an error such as "The Exchange Connector version is not supported" when attempting to set up the Exchange connector.</span></span> <span data-ttu-id="f5be3-107">Mi lehet az oka?</span><span class="sxs-lookup"><span data-stu-id="f5be3-107">What could be the cause?</span></span>

<span data-ttu-id="f5be3-108">A: a használt fiók megfelelő licenccel rendelkezik – aktív Intune licenccel kell rendelkeznie.</span><span class="sxs-lookup"><span data-stu-id="f5be3-108">A: The account you are using is licensed appropriately - it must have an active Intune license</span></span>

<span data-ttu-id="f5be3-109">K: lehet több Exchange összekötőt is?</span><span class="sxs-lookup"><span data-stu-id="f5be3-109">Q: Is it possible to have multiple Exchange connectors?</span></span>

<span data-ttu-id="f5be3-110">A: csak egyetlen Exchange-csatlakozót állíthat be egy Intune-bérlői fiókhoz egy Exchange-szervezetben.</span><span class="sxs-lookup"><span data-stu-id="f5be3-110">A: You can only set up one Exchange connector per Intune tenant per Exchange organization.</span></span> <span data-ttu-id="f5be3-111">Az összekötő csak egy kiszolgálón telepíthető több kiszolgálós Exchange-szervezetben.</span><span class="sxs-lookup"><span data-stu-id="f5be3-111">The connector can only be installed on one server in a multi server exchange organization.</span></span>

<span data-ttu-id="f5be3-112">Az egyazon bérlői fiókban konfigurált Exchange-és Exchange Online-kapcsolatokhoz is nincs konfigurálva az összekötők.</span><span class="sxs-lookup"><span data-stu-id="f5be3-112">Also you cannot have connectors configured for both Exchange on-premise and Exchange Online configured in the same tenant.</span></span>

<span data-ttu-id="f5be3-113">K: használhatók-e az összekötők CAS-tömbökkel az Exchange-kapcsolaton keresztül?</span><span class="sxs-lookup"><span data-stu-id="f5be3-113">Q: Can the connector use a CAS array as its connection to Exchange?</span></span>

<span data-ttu-id="f5be3-114">A: a CAS-tömb megadása nem támogatott konfiguráció az összekötő beállításai között.</span><span class="sxs-lookup"><span data-stu-id="f5be3-114">A: Specifying a CAS array is not a supported configuration in the connector setup.</span></span> <span data-ttu-id="f5be3-115">Csak egyetlen kiszolgálót kell megadni, és az összekötő konfigurációs fájlban kell hardcoded, amely megtalálható</span><span class="sxs-lookup"><span data-stu-id="f5be3-115">Only a single server should be specified and should be hardcoded in the connector configuration file which can be found in</span></span>

<span data-ttu-id="f5be3-116">program data\microsoft\microsoft Intune a helyi Exchange-csatlakozón \ OnpremiseExchangeConnectorServiceConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="f5be3-116">program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml</span></span>

<span data-ttu-id="f5be3-117">Keresse meg a következő bejegyzést ```<ExchangeWebServiceURL />``` , és cserélje le az URL-t az Exchange-kiszolgálóval.</span><span class="sxs-lookup"><span data-stu-id="f5be3-117">Locate the following entry ```<ExchangeWebServiceURL />``` and replace the URL with the exchange server.</span></span>

<span data-ttu-id="f5be3-118">**Például**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span><span class="sxs-lookup"><span data-stu-id="f5be3-118">**Example:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span></span>

<span data-ttu-id="f5be3-119">További hibaelhárítási információkat az alábbi dokumentációban talál: [Intune helyszíni Exchange-összekötő hibaelhárítása](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span><span class="sxs-lookup"><span data-stu-id="f5be3-119">Please see the following documentation for additional troubleshooting: [Troubleshoot the Intune on-premises Exchange connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span></span>

<span data-ttu-id="f5be3-120">**Az Exchange összekötő részletes naplózásának engedélyezése**</span><span class="sxs-lookup"><span data-stu-id="f5be3-120">**Enabling Verbose logging for the Exchange connector**</span></span>

1. <span data-ttu-id="f5be3-121">Nyissa meg szerkesztésre az Exchange Connector-nyomkövetési konfigurációs fájlt.</span><span class="sxs-lookup"><span data-stu-id="f5be3-121">Open the Exchange Connector tracing configuration file for editing.</span></span>  
<span data-ttu-id="f5be3-122">A fájl a következő helyen található:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="f5be3-122">The file is located at : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span></span>  

<span data-ttu-id="f5be3-123">**Például**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span><span class="sxs-lookup"><span data-stu-id="f5be3-123">**Example:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span></span>
  
2. <span data-ttu-id="f5be3-124">Keresse meg a TraceSourceLine a következő kulccsal: OnPremisesExchangeConnectorService</span><span class="sxs-lookup"><span data-stu-id="f5be3-124">Locate the TraceSourceLine with the following key: OnPremisesExchangeConnectorService</span></span>  
  
3. <span data-ttu-id="f5be3-125">A SourceLevel csomópont értékének módosítása az adatok ActivityTracing (az alapértelmezett) a bőbeszédű ActivityTracing</span><span class="sxs-lookup"><span data-stu-id="f5be3-125">Change the SourceLevel node value from Information ActivityTracing (the default) to Verbose ActivityTracing</span></span>  

<span data-ttu-id="f5be3-126">**Például**</span><span class="sxs-lookup"><span data-stu-id="f5be3-126">**Example:**</span></span>
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
4. <span data-ttu-id="f5be3-127">A Microsoft Intune Exchange szolgáltatás újraindítása</span><span class="sxs-lookup"><span data-stu-id="f5be3-127">Restart the Microsoft Intune Exchange Service</span></span>  
5. <span data-ttu-id="f5be3-128">Teljes szinkronizálás az Intune-portálon, amíg el nem fejeződik, majd az XML visszaváltása "információs ActivityTracing", majd indítsa újra a Microsoft Intune Exchange szolgáltatást.</span><span class="sxs-lookup"><span data-stu-id="f5be3-128">Full sync in Intune Portal until it finishes and then change the XML back to "Information ActivityTracing" and restart the Microsoft Intune Exchange Service.</span></span>  
6. <span data-ttu-id="f5be3-129">A naplók helye: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span><span class="sxs-lookup"><span data-stu-id="f5be3-129">Location of the logs is : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span></span>