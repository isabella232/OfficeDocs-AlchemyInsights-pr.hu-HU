---
title: A TLS1.0 és a TLS 1.1 letiltása az SMTP AUTH-ügyfélküldéshez
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13649"
- "9005383"
ms.openlocfilehash: 6751f4e8a177958fdec674899606252a4ae40a72
ms.sourcegitcommit: d9e6f700cd73a61c109e2a99bc71e559dba34722
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/18/2021
ms.locfileid: "58454772"
---
# <a name="disabling-tls10-and-tls-11-for-smtp-auth-client-submission"></a>A TLS1.0 és a TLS 1.1 letiltása az SMTP AUTH-ügyfélküldéshez

Nemrégiben letiltottük a TLS1.0 és a TLS 1.1 protokollt az SMTP AUTH-ügyfélküldéshez. 

Ha olyan eszközt, alkalmazást vagy kiszolgálót konfigurált, amely az SMTP AUTH Microsoft 365 küldési módszerrel küld e-maileket az Microsoft 365, ellenőrizze, hogy az eszköz, alkalmazás vagy kiszolgáló támogatja-e a TLS 1.2-es smtp-t. 