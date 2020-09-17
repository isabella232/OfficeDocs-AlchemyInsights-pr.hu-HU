---
title: a 1065 EOP kimenő IP-címek rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806797"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="daec6-102">A kimenő IP-címtartományok EOP megszűnése</span><span class="sxs-lookup"><span data-stu-id="daec6-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="daec6-103">A szervezetével kapcsolatos esetleges problémát észlelt, amely (ha az 2018 október 26-ának nincs kijavítva) az e-mailek áramlását a helyszíni vagy a külső célállomásokra is megszakíthatja.</span><span class="sxs-lookup"><span data-stu-id="daec6-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="daec6-104">A korábban közölt módon az IP-címtartomány-kezelés egyszerűsítése érdekében a Microsoft 365-on kívüli e-mailek küldéséhez és átvételéhez használt Exchange Online Protection (EOP) IP-címtartományok egységesítése.</span><span class="sxs-lookup"><span data-stu-id="daec6-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="daec6-105">Az elemzés azt jelzi, hogy az e-mail-forgalom összekötői között konfigurált külső e-mail-források vagy-célhelyek közül legalább az [itt](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)látható IP-címtartományból származó kapcsolatokat fogadja.</span><span class="sxs-lookup"><span data-stu-id="daec6-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="daec6-106">Október 26-án, annak biztosítása érdekében, hogy ezek a források és a rendeltetési hely az összes [közzétett EOP-](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)címről kapcsolatot fogadjon.</span><span class="sxs-lookup"><span data-stu-id="daec6-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="daec6-107">Ha további információra van kíváncsi a változásról, olvassa el a [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), a [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)vagy a [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="daec6-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="daec6-108">**Megjegyzés**: Ha korábban már használta az IP-címet vagy az URL-címet HTML-, XML-és RSS-en keresztül, akkor az új webes szolgáltatásokra kell áttérnie az ilyen típusú frissítések automatizálásához.</span><span class="sxs-lookup"><span data-stu-id="daec6-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="daec6-109">További információt a [microsoft 365-végpontok kategóriái és a microsoft 365 IP-cím és URL-webszolgáltatás](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)című témakörben találhat.</span><span class="sxs-lookup"><span data-stu-id="daec6-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
