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
ms.openlocfilehash: 85cbd89e461f36a51eed816619fd132ea60dfdb0014eb850c7ec3f38d41e1ca2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069966"
---
# <a name="conditional-access-issues"></a>A feltételes hozzáféréssel kapcsolatos problémák

**A bejelentkezési diagnosztika problémáinak megoldása**

A bejelentkezés diagnosztikai eszközével gyorsan kiderítheti, hogy mi történt, vagy diagnosztizálhatja a felhasználói [bejelentkezéssel kapcsolatos problémákat:](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Indítsa el a Bejelentkezés diagnosztikát.
1. Keresse meg az elemezni szükséges eseményt a felhasználóval, alkalmazással, a bejelentkezés időpontjával, a kérelem azonosítójával vagy a korrelációs azonosítóval kapcsolatos részletek megadásával.
1. Tekintse át a diagnosztikai eredményeket, és nézze meg, hogy mi történt, és milyen műveleteket lehet tenni a módosításokhoz (ha szükség van módosításokra).

**Steps to Troubleshoot a Sign-In** 

1. Lépjen az Azure AD Bejelentkezési lapra.
1. A bejelentkezéseket szűrheti felhasználó, időtartomány, alkalmazás, állapot, ügyfélalkalmazás stb. szerint.
1. Válasszon ki egy bejelentkezési eseményt, és tekintse meg a Feltételes hozzáférés lapot a kiértékelt házirendek megtekintéséhez.
1. A házirend részleteinek megtekintéséhez és az alkalmazás okának megtekintéséhez kattintson a házirend sorra.

**Tools to troubleshoot a Conditional Access policy**

- A csak jelentés módban a felhasználók befolyásolása nélkül értékelheti ki a házirendeket.
- A What-if eszközzel szimulálhatja a bejelentkezési eseményeket, és láthatja, hogy milyen házirendek vonatkoznak rá.
- Elemzések és jelentéskészítési munkafüzetben valós időben jelenik meg az egyes házirendek hatása.

**Alaptervvédelmi szabályzatok**

Az Alaptervvédelmi házirendek elavultak. Többé nem érvényesíti őket a rendszer, és hamarosan eltávolítjuk őket az Azure Portalról. Azt javasoljuk, hogy [engedélyeznie kell a biztonsági alapértelmezett értékeket.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)

További információ a feltételes hozzáférésről:

[Gyakorlati tanácsok a feltételes hozzáféréshez Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Feltételek a feltételes hozzáférésben](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Controls in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Helyek a feltételes hozzáférésben](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
