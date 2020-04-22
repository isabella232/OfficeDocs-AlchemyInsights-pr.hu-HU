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
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>EOP kimenő IP-címtartományok eprektálása

Észleltünk egy lehetséges problémát a szervezetnél, amely (ha nem javítja ki 2018. október 26-ig) megszakíthatja a helyszíni vagy külső célállomásokra irányuló levélforgalmat. Ahogy azt korábban közöltük, az IP-címtartomány kezelésének egyszerűsítése érdekében konszolidáljuk az Exchange Online Protection (EOP) IP-címtartományait, amelyek a Microsoft 365-ön kívüli e-mailek küldésére és fogadására szolgálnak. Elemzésünk azt mutatja, hogy a levelezési összekötőkben konfigurált külső e-mail források vagy célállomások közül egy vagy több nem fogad kapcsolatot az [itt](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)látható IP-címtartományokból.

Törvény előtt október 26 annak biztosítása érdekében, ezek a források és célok elfogadja kapcsolatok és az összes [közzétett EOP IP-címek](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

A változásról további információt az [MC146155,](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155) [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)vagy [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)állások üzenetközpontban talál.

**Megjegyzés:** Ha korábban HTML-, XML- és RSS-alapú IP-cím- vagy URL-közzétételt használt a végpontfrissítésekhez, akkor az ilyen típusú frissítések automatizálásához át kell térnie az új webszolgáltatásokra is. További információt a [Microsoft 365 végpontkategóriák és a Microsoft 365 IP-cím és URL-cím webszolgáltatás című témakörben talál.](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)
