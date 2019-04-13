---
title: 1065 kapcsolójáról EOP kimenő IP-cím rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 17beb1722142d94ea05b67ce5ed1f20f8b11375c
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/13/2019
ms.locfileid: "31858098"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="c3cae-102">Kimenő IP-címtartományok EOP kapcsolójáról</span><span class="sxs-lookup"><span data-stu-id="c3cae-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="c3cae-103">A problémát a szervezet, amely (Ha nem javítja ki a 2018. október 26.) üzenetkezelési megszakíthatja a helyszíni vagy a külső hivatkozási helyekre is található.</span><span class="sxs-lookup"><span data-stu-id="c3cae-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="c3cae-104">Mint korábban közölt egyszerűsítése érdekében az IP-címek tartományának kezelése azt összesítést végzünk, az Exchange Online Protection (EOP) IP-címtartományokat, küldhet és fogadhat e-mail Office 365 kívül használt.</span><span class="sxs-lookup"><span data-stu-id="c3cae-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365.</span></span> <span data-ttu-id="c3cae-105">Az elemzés azt jelzi, hogy egy vagy több e-mail külső források vagy célok mail áramlási összekötők beállított kapcsolatokat az IP cím tartomány látható [Itt](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)nem fogad.</span><span class="sxs-lookup"><span data-stu-id="c3cae-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="c3cae-106">Október 26, annak biztosítása érdekében, hogy ezeket a forrásokat és célokat elfogadja a kapcsolatok és az összes [közzétett EOP IP-címek](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)előtt eljárni.</span><span class="sxs-lookup"><span data-stu-id="c3cae-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="c3cae-107">Ez a módosítás kapcsolatos további tudnivalókért tanulmányozza Message Center könyveli, [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)vagy [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="c3cae-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="c3cae-108">**Megjegyzés**: korábban használt IP- vagy URL-cím közzétételi keresztül HTML, XML és RSS végpont frissítések, ha is át kell telepítenie, az új webes szolgáltatások ilyen típusú frissítéseket automatizálása.</span><span class="sxs-lookup"><span data-stu-id="c3cae-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="c3cae-109">További információt talál az [Office 365 végpont kategóriák és az Office 365 IP-cím és a webszolgáltatás URL-címe](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="c3cae-109">For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
