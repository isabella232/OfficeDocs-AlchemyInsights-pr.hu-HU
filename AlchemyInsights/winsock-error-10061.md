---
title: 1554 Winsock-hiba 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698864"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="f976c-102">WINSOCK-hiba 10061</span><span class="sxs-lookup"><span data-stu-id="f976c-102">Winsock error 10061</span></span>

<span data-ttu-id="f976c-103">Ez a hibakód azt jelzi, hogy a Microsoft nem tudott TCP-szoftvercsatornát (kapcsolatot) létesíteni a célállomással.</span><span class="sxs-lookup"><span data-stu-id="f976c-103">This error code means that Microsoft couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="f976c-104">A hiba legvalószínűbb oka a tűzfal-konfigurációval kapcsolatos probléma.</span><span class="sxs-lookup"><span data-stu-id="f976c-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="f976c-105">A probléma megoldásához tekintse át a következő beállításokat:</span><span class="sxs-lookup"><span data-stu-id="f976c-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="f976c-106">Tűzfal-konfiguráció ellenőrzése a [Microsoft 365 URL-címei és IP-címei](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges) szerinti adatokkal</span><span class="sxs-lookup"><span data-stu-id="f976c-106">Verify your firewall configuration with the information in [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="f976c-107">Ha a hiba az Exchange Online védelmi szolgáltatással (EOP) függ, korábban értesítést kellett volna küldenie az [Exchange Online védelmi szolgáltatás IP-címeinek](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)módosításáról.</span><span class="sxs-lookup"><span data-stu-id="f976c-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="f976c-108">Ellenőrizze, hogy az INTERNETSZOLGÁLTATÓja nem blokkolja-e a portot.</span><span class="sxs-lookup"><span data-stu-id="f976c-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="f976c-109">Ellenőrizze az összekötők intelligens állomás-és célkiszolgáló-beállításait.</span><span class="sxs-lookup"><span data-stu-id="f976c-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="f976c-110">Fontos tudni, hogy a Microsoft 365 ilyen módon nem blokkolja a *bejövő* kapcsolatokat.</span><span class="sxs-lookup"><span data-stu-id="f976c-110">Note that Microsoft 365 doesn't block *incoming* connections in this manner.</span></span>
