---
title: E-mail-továbbítás a Microsoft 365-ön keresztül
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 3b07dd4ccc8570e77a9ce30df48f9ac987a1db71
ms.sourcegitcommit: 93292c46464ac94971d11adfb808d066ab8bc406
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53117985"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>Többfunkciós eszköz vagy alkalmazás beállítása levelek küldéséhez

A különféle lehetőségekről és az eljárás lépéseiről a [Többfunkciós eszköz vagy alkalmazás beállítása a Microsoft 365-tel való levelezéshez](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365) című cikk nyújt tájékoztatást.
  
Ha olyan eszköze vagy alkalmazása van, amely nemrég leállt, a leggyakoribb problémák a következők:

- **Hitelesítéssel kapcsolatos hibák AZ SMTP Auth-ügyfélküldés használata során** Nemrégiben megváltoztattunk néhány, az SMTP-hitelesítés működését. A problémák megoldásával kapcsolatos további információkért lásd: Az e-maileket levelező nyomtatókkal, szkennerekkel és hálózatolvasókkal kapcsolatos problémák megoldása a hitelesítés sikertelen Microsoft 365 [vagy](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)Office 365.
- **A TLS 1.2-es** verzióját fogadjuk el, miközben biztonságos kapcsolatot létesítünk Office 365 Biztonságos kapcsolat (TLS) használata esetén győződjön meg arról, hogy az alkalmazáseszköz támogatja a TLS 1.2-es adatokat. További információt a Felkészülés a [TLS 1.2-esre](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)a Office 365 és a Office 365 GCC.
 
Más problémákról és megoldásokról Az e-maileket levelező [nyomtatók,](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)szkennerek éslobrák problémáinak megoldása Microsoft 365 vagy Office 365.

Az érintett eszközök megjelenítéséhez nyissa meg az [SMTP-hitelesítést használó ügyfelekről szóló jelentést](https://protection.office.com/mailflow/dashboard).

**Megjegyzés:** Exchange Online tömeges levelezési esetek nem használhatók. Ha tömeges kereskedelmi e-maileket (például ügyfél hírleveleket) is el kell küldenie, külső szolgáltatót kell használnia, amely ezekre a szolgáltatásokra specializál.
