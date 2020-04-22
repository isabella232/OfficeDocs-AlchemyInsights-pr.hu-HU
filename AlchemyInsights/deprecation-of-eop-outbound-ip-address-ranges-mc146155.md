---
title: 1065 Az EOP kimenő IP-címtartományainak eprecation-jaMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: f4854c32d970d84f3a0664a9e384dc6e3cd0bfa7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704599"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="aa99a-102">EOP kimenő IP-címtartományok eprektálása</span><span class="sxs-lookup"><span data-stu-id="aa99a-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="aa99a-103">Észleltünk egy lehetséges problémát a szervezetnél, amely (ha nem javítja ki 2018. október 26-ig) megszakíthatja a helyszíni vagy külső célállomásokra irányuló levélforgalmat.</span><span class="sxs-lookup"><span data-stu-id="aa99a-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="aa99a-104">Ahogy azt korábban közöltük, az IP-címtartomány kezelésének egyszerűsítése érdekében konszolidáljuk az Exchange Online Protection (EOP) IP-címtartományait, amelyek a Microsoft 365-ön kívüli e-mailek küldésére és fogadására szolgálnak.</span><span class="sxs-lookup"><span data-stu-id="aa99a-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="aa99a-105">Elemzésünk azt mutatja, hogy a levelezési összekötőkben konfigurált külső e-mail források vagy célállomások közül egy vagy több nem fogad kapcsolatot az [itt](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)látható IP-címtartományokból.</span><span class="sxs-lookup"><span data-stu-id="aa99a-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="aa99a-106">Törvény előtt október 26 annak biztosítása érdekében, ezek a források és célok elfogadja kapcsolatok és az összes [közzétett EOP IP-címek](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="aa99a-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="aa99a-107">A változásról további információt az [MC146155,](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155) [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)vagy [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)állások üzenetközpontban talál.</span><span class="sxs-lookup"><span data-stu-id="aa99a-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="aa99a-108">**Megjegyzés:** Ha korábban HTML-, XML- és RSS-alapú IP-cím- vagy URL-közzétételt használt a végpontfrissítésekhez, akkor az ilyen típusú frissítések automatizálásához át kell térnie az új webszolgáltatásokra is.</span><span class="sxs-lookup"><span data-stu-id="aa99a-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="aa99a-109">További információt a [Microsoft 365 végpontkategóriák és a Microsoft 365 IP-cím és URL-cím webszolgáltatás című témakörben talál.](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)</span><span class="sxs-lookup"><span data-stu-id="aa99a-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
