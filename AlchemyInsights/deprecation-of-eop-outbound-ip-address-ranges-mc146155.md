---
title: 1065 Az EOP kimenő IP-címtartományának elavultaMC146155
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
ms.openlocfilehash: 214abc57a99c70a02a7d159441713e007f6ad980f67e373780d4ca297f69f764
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031264"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Kimenő EOP-címtartományok elavultak

Észleltünk egy lehetséges problémát a szervezetében, amely (ha nem javítja ki 2018. október 26-ig) megszakíthatja az e-mailek helyszíni vagy külső célhelyre való áramlását. Ahogy azt korábban említettük, az IP-címtartomány-kezelés egyszerűsítése érdekében összevonjuk az Exchange Online Védelmi szolgáltatás (EOP) IP-címtartományát, amely az e-mailek külső küldését és fogadását Microsoft 365. Elemzésünk szerint az e-mail-forgalom összekötőiben beállított külső e-mail-források vagy célhelyek egyike vagy többe [](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)nem fogad kapcsolatokat az itt látható IP-címtartományból.

Október 26-a előtt járjon el annak érdekében, hogy ezek a források és célhelyek minden [közzétett EOP-IP-címhez](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)és címről fogadjanak el kapcsolatokat.

A változásról további információt az Üzenetközpont bejegyzései [MC146155,](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155) [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)vagy [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Megjegyzés:** Ha korábban HTML, XML és RSS protokollon keresztüli IP- vagy URL-közzétételt használt a végpontok frissítéséhez, akkor az ilyen típusú frissítések automatizálására is át kell telepítenie az új webes szolgáltatásokat. További információt a Végpontkategóriák Microsoft 365 és az [IP-Microsoft 365](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)URL-webszolgáltatással kapcsolatban.
