---
title: 1554 Winsock hiba 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: f54c7fc81c274871fbc22908ce0fb21500975d9e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530796"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="4bfad-102">Winsock hiba 10061</span><span class="sxs-lookup"><span data-stu-id="4bfad-102">Winsock error 10061</span></span>

<span data-ttu-id="4bfad-103">Ez a hibakód azt jelenti, hogy Office 365 nem tudta létrehozni a TCP-szoftvercsatornát (kapcsolat) és a célállomás.</span><span class="sxs-lookup"><span data-stu-id="4bfad-103">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="4bfad-104">A hiba legvalószínűbb oka a tűzfal konfigurációs probléma.</span><span class="sxs-lookup"><span data-stu-id="4bfad-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="4bfad-105">A probléma megoldásához ellenőrizze ezeket a beállításokat:</span><span class="sxs-lookup"><span data-stu-id="4bfad-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="4bfad-106">Az [Office 365 URL-címek és IP-címtartományokat](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges) adatokkal a tűzfal konfigurációjának ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="4bfad-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="4bfad-107">A hiba esetén az Exchange Online Protection (EOP) adott kell korábban értesítést kapott a módosítása az [Exchange Online védelem IP-címeket](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="4bfad-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="4bfad-108">Győződjön meg arról, hogy az internetszolgáltató (ISP) nem blokkolja azt a portot.</span><span class="sxs-lookup"><span data-stu-id="4bfad-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="4bfad-109">Ellenőrizze az intelligens állomás és a cél kiszolgáló beállításai az összekötők.</span><span class="sxs-lookup"><span data-stu-id="4bfad-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="4bfad-110">Fontos megjegyezni, hogy Office 365 nem blokkolja a *bejövő* kapcsolatok ily módon.</span><span class="sxs-lookup"><span data-stu-id="4bfad-110">Note that Office 365 doesn't block *incoming* connections in this manner.</span></span>
