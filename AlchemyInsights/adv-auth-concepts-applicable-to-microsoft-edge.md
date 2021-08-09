---
title: Speciális hitelesítési fogalmak a Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: 8ddec37260ec4e3bcc390dcc8adb7397368de19555ee31be458be033d3886386
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934367"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Speciális hitelesítési fogalmak a Microsoft Edge

Az alábbiakban a hitelesítésre vonatkozó speciális fogalmakat Microsoft Edge:

**Proaktív hitelesítés**

Amikor engedélyezi a [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) házirendet, a Microsoft Edge megpróbálja proaktívan hitelesíteni a bejelentkezett felhasználókat a Microsoft-szolgáltatások. Rendszeres időközönként egy online szolgáltatáson keresztül ellenőrzi a proaktív hitelesítést szabályozó konfigurációt tartalmazó frissített jegyzékfájlt.

Előnyök: A proaktív hitelesítés lehetővé teszi a hitelesítést a főbb szolgáltatásoknak, például az Office lapnak. Ha a Bing keresőmotorként használja, a proaktív hitelesítés javítja a címsor teljesítményét, és a vállalat igényeire szabott keresési eredményeket hoz létre.

**Windows Hello CredUI for NTLM Authentication**

Ha az egyszeri bejelentkezés nem érhető el, amikor egy webhely ntLM vagy egyeztetési mechanizmuson keresztül próbál meg bejelentkezni a felhasználóba, ez a szolgáltatás lehetővé teszi, hogy a felhasználó megosztsa az operációs rendszer hitelesítő adatait a webtel, és megfeleljen Windows Hello tanúsítványos felhasználói felület használatával Windows Hello hitelesítési kihívásnak. Ez a bejelentkezési folyamat csak a Windows 10 és csak az olyan felhasználóknál jelenik meg, akik nem kapják meg az SSO-t NTLM vagy a Negotiate kihívás során.

**Mentett jelszavak használata az automatikus bejelentkezéshez**

Azok a felhasználók, akik jelszavakat Microsoft Edge engedélyezhetik az automatikus bejelentkezést olyan webhelyekre, amelyekhez hitelesítő adatokat mentettek. A felhasználók be- vagy kikapcsolhatja ezt a edge://settings/passwords, és a jelszókezelői [házirendek között is konfigurálhatja.](https://go.microsoft.com/fwlink/?linkid=2134622)
