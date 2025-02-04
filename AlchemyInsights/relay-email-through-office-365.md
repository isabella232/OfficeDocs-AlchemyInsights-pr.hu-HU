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
ms.openlocfilehash: f02daad7d4b4a11f8d8bb1ef1467db5809cbd291
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324364"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>Többfunkciós eszköz vagy alkalmazás beállítása levelek küldéséhez

A különféle lehetőségekről és az eljárás lépéseiről a [Többfunkciós eszköz vagy alkalmazás beállítása a Microsoft 365-tel való levelezéshez](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365) című cikk nyújt tájékoztatást.
  
Ha olyan eszköze vagy alkalmazása van, amely nemrég leállt, a leggyakoribb problémák a következők:

- **Hitelesítéssel kapcsolatos hibák AZ SMTP Auth-ügyfélküldés használata során** Nemrégiben megváltoztattunk néhány, az SMTP-hitelesítés működését. A problémák megoldásával kapcsolatos további információkért lásd: Az e-maileket levelező nyomtatókkal, szkennerekkel és hálózatolvasókkal kapcsolatos problémák megoldása a hitelesítés sikertelen Microsoft 365 [vagy](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)Office 365.
- **A TLS 1.2-es** verzióját fogadjuk el, miközben biztonságos kapcsolatot létesítünk Office 365 Biztonságos kapcsolat (TLS) használata esetén győződjön meg arról, hogy az alkalmazáseszköz támogatja a TLS 1.2-es adatokat. További információt a Felkészülés a [TLS 1.2-esre](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)a Office 365 és a Office 365 GCC.
 
Más problémákról és megoldásokról Az e-maileket levelező [nyomtatókkal,](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)szkennerekkel éslobbanás alkalmazásokkal kapcsolatos problémák megoldása Microsoft 365 vagy Office 365.

Az érintett eszközök megjelenítéséhez nyissa meg az [SMTP-hitelesítést használó ügyfelekről szóló jelentést](https://protection.office.com/mailflow/dashboard).

**Megjegyzés:** Exchange Online a tömeges levelezési esetek nem használhatók. Ha tömeges kereskedelmi e-maileket (például ügyfél hírleveleket) is el kell küldenie, külső szolgáltatót kell használnia, amely ezekre a szolgáltatásokra specializál.
