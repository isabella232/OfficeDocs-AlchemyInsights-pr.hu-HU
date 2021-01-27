---
title: A feltételes hozzáféréssel kapcsolatos problémák
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014883"
---
# <a name="conditional-access-issues"></a>A feltételes hozzáféréssel kapcsolatos problémák

**A bejelentkezés diagnosztikai problémáinak megoldása**

A bejelentkezés diagnosztikai eszközével gyorsan kiderítheti, hogy mi történt, vagy diagnosztizálhatja a felhasználói [bejelentkezéssel kapcsolatos problémákat:](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Indítsa el a bejelentkezés diagnosztikai eszközét.
1. Keresse meg az elemezni szükséges eseményt a felhasználóval, alkalmazással, a bejelentkezés időpontjával, a kérelem azonosítójával vagy a korrelációs azonosítóval kapcsolatos adatok megadásával.
1. Tekintse át a diagnosztikai eredményeket, amelyekben látható a hiba részletei, valamint a módosításokhoz szükséges műveletek (ha szükséges).

**A bejelentkezési hibák elhárításának lépései** 

1. Nyissa meg az Azure AD bejelentkezési lapját.
1. A bejelentkezések szűrése felhasználó, időtartomány, alkalmazás, állapot, ügyfélalkalmazás stb. szerint.
1. Jelöljön ki egy bejelentkezési eseményt, és tekintse meg a Feltételes hozzáférés lapot a kiértékelt házirendek megtekintéséhez.
1. Kattintson egy házirend sorra a házirend részleteinek megtekintéséhez és annak okának megtekintéséhez.

**A feltételes hozzáférésre vonatkozó házirendek hibaelhárítási eszközei**

- A csak jelentés módban a felhasználók befolyásolása nélkül értékelheti ki a házirendeket.
- A "mi van, ha" eszközzel szimulálhatja a bejelentkezési eseményeket, és megtekintheti, hogy mely házirendek érvényesek.
- A Betekintések és jelentéskészítési munkafüzet valós időben jeleníti meg az egyes házirendeket.

**Alaptervvédelmi házirendek**

Az Alaptervvédelmi házirendek elavultak. A továbbiakban nem érvényesíti őket a rendszer, és hamarosan el is távolítjuk őket az Azure Portalról. Azt javasoljuk, hogy [engedélyezi a biztonsági alapértelmezett beállításokat.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)

A feltételes hozzáféréssel kapcsolatos további információkért lásd:

[Gyakorlati tanácsok az Azure Active Directory feltételes hozzáféréshez](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Feltételek a feltételes hozzáférésben](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Vezérlők a feltételes hozzáférésben](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Helyek a feltételes hozzáférésben](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
