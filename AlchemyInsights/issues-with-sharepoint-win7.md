---
title: A 7 SharePoint gépre Windows problémák
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
- "9006484"
- "11070"
ms.openlocfilehash: 787f0e713cc95b590bc494868d5098a25131ac56
ms.sourcegitcommit: d33ab8c73d8af51da782094fb8f8abf7626f4df3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52125122"
---
# <a name="issues-with-sharepoint-on-windows-7-machines"></a>A 7 SharePoint gépre Windows problémák

Ha Windows 7 gépén hibaüzenetet kap, miközben SharePoint vagy OneDrive-on dolgozik, azok a TLS 1.0/1.1-es hiba elavultságával függnek fel. További információ:

- [Felkészülés a TLS 1.2-re az Office 365-ben és az Office 365 GCC-ben](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- Windows 7 SP1/Windows 8-ügyfélnek engedélyezve kell lennie a TLS1.2-nek. További információ: Hitelesítési hibák olyankor, amikor az ügyfél nem támogatja a [TLS 1.2-es használatát.](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- Telepítse a KB3140245-öt, és hozza létre a beállításjegyzékbeli értéket. További információt a Frissítés a [TLS 1.1 és a TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392) alapértelmezett biztonságos protokollként való engedélyezéséhez a Windows winhttps://Windows

- Windows 7 SP1/Windows 8 ügyfélnek gondoskodnia kell arról, hogy a legújabb TLS-rejtjelcsomagok telepítve vannak. További információ: [Microsoft biztonsági tanácsadó 3042058.](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058) 


