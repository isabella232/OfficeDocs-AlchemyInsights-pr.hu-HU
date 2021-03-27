---
title: A Microsoft Edge speciális hitelesítési koncepciói
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
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398586"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>A Microsoft Edge speciális hitelesítési koncepciói

Az alábbiakban a Microsoft Edge-re vonatkozó speciális hitelesítési fogalmakat íme:

**Proaktív hitelesítés**

A [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) házirend engedélyezésekor a Microsoft Edge megpróbálja proaktívan hitelesíteni a bejelentkezett felhasználókat a Microsoft-szolgáltatásokon keresztül. Rendszeres időközönként egy online szolgáltatáson keresztül ellenőrzi a proaktív hitelesítést szabályozó konfigurációt tartalmazó frissített jegyzékfájlt.

Előnyök: A proaktív hitelesítés hitelesítést tesz lehetővé a főbb szolgáltatásoknak, például az Office Új lapnak. Ha keresőmotorként a Binget használja, a proaktív hitelesítés javítja a címsor teljesítményét, és a vállalat igényeire szabott keresési eredményeket hoz létre.

**Windows Hello CredUI NTLM-hitelesítéshez**

Ha az egyszeri bejelentkezés nem érhető el, amikor egy webhely az NTLM vagy a Egyeztetési mechanizmuson keresztül próbál meg bejelentkezni a felhasználóba, ez a funkció lehetővé teszi, hogy a felhasználó megosztsa az operációs rendszer hitelesítő adatait a webtel, és megfeleljön a hitelesítési kihívásnak a Windows Hello Cred felhasználói felület használatával. Ez a bejelentkezési folyamat csak a Windows 10-ben fog megjelenni, és csak azok a felhasználók számára, akik nem kapják meg az SSO-t NTLM vagy a negotiate challenge (Kienálás).

**Mentett jelszavak használata az automatikus bejelentkezéshez**

Azok a felhasználók, akik jelszavakat mentnek a Microsoft Edge-ben, engedélyezhetik az automatikus bejelentkezést olyan webhelyekre, amelyekhez hitelesítő adatokat mentettek. A felhasználók be- vagy kikapcsolhatja ezt a edge://settings/passwords, és a jelszókezelői [házirendek között is konfigurálhatja.](https://go.microsoft.com/fwlink/?linkid=2134622)
