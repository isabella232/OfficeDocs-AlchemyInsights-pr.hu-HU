---
title: 1554 Winsock hiba 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 9331a6c2b6e92a66fb97daf7dc5655ec320cba0f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29903101"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="5dbb5-102">Winsock hiba 10061</span><span class="sxs-lookup"><span data-stu-id="5dbb5-102">Winsock error 10061</span></span>

<span data-ttu-id="5dbb5-p101">Ez a hibakód azt jelenti, hogy Office 365 nem tudta létrehozni a TCP-szoftvercsatornát (kapcsolat) és a célállomás. A hiba legvalószínűbb oka a tűzfal konfigurációs probléma. A probléma megoldásához ellenőrizze ezeket a beállításokat:</span><span class="sxs-lookup"><span data-stu-id="5dbb5-p101">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host. The most likely cause of this error is a problem with your firewall configuration. To fix the problem, check these settings:</span></span>
  
- <span data-ttu-id="5dbb5-106">Az [Office 365 URL-címek és IP-címtartományokat](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges) adatokkal a tűzfal konfigurációjának ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="5dbb5-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>
    
- <span data-ttu-id="5dbb5-107">A hiba esetén az Exchange Online Protection (EOP) adott kell korábban értesítést kapott a módosítása az [Exchange Online védelem IP-címeket](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="5dbb5-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
    
- <span data-ttu-id="5dbb5-108">Győződjön meg arról, hogy az internetszolgáltató (ISP) nem blokkolja azt a portot.</span><span class="sxs-lookup"><span data-stu-id="5dbb5-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>
    
- <span data-ttu-id="5dbb5-109">Ellenőrizze az intelligens állomás és a cél kiszolgáló beállításai az összekötők.</span><span class="sxs-lookup"><span data-stu-id="5dbb5-109">Verify the smart host and target server settings in your connectors.</span></span>
    
<span data-ttu-id="5dbb5-110">Fontos megjegyezni, hogy Office 365 nem blokkolja a *bejövő* kapcsolatok ily módon.</span><span class="sxs-lookup"><span data-stu-id="5dbb5-110">Note that Office 365 doesn't block  *incoming*  connections in this manner.</span></span> 
  

