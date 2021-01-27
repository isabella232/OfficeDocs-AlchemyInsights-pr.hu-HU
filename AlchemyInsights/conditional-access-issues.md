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
# <a name="conditional-access-issues"></a><span data-ttu-id="637a2-102">A feltételes hozzáféréssel kapcsolatos problémák</span><span class="sxs-lookup"><span data-stu-id="637a2-102">Conditional access issues</span></span>

<span data-ttu-id="637a2-103">**A bejelentkezés diagnosztikai problémáinak megoldása**</span><span class="sxs-lookup"><span data-stu-id="637a2-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="637a2-104">A bejelentkezés diagnosztikai eszközével gyorsan kiderítheti, hogy mi történt, vagy diagnosztizálhatja a felhasználói [bejelentkezéssel kapcsolatos problémákat:](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="637a2-104">You can quickly find out what happened or diagnose problems related to user sign-in by using the [Sign-in Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span></span>

1. <span data-ttu-id="637a2-105">Indítsa el a bejelentkezés diagnosztikai eszközét.</span><span class="sxs-lookup"><span data-stu-id="637a2-105">Launch the Sign-in Diagnostic.</span></span>
1. <span data-ttu-id="637a2-106">Keresse meg az elemezni szükséges eseményt a felhasználóval, alkalmazással, a bejelentkezés időpontjával, a kérelem azonosítójával vagy a korrelációs azonosítóval kapcsolatos adatok megadásával.</span><span class="sxs-lookup"><span data-stu-id="637a2-106">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="637a2-107">Tekintse át a diagnosztikai eredményeket, amelyekben látható a hiba részletei, valamint a módosításokhoz szükséges műveletek (ha szükséges).</span><span class="sxs-lookup"><span data-stu-id="637a2-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes (if any changes are needed).</span></span>

<span data-ttu-id="637a2-108">**A bejelentkezési hibák elhárításának lépései**</span><span class="sxs-lookup"><span data-stu-id="637a2-108">**Steps to Troubleshoot a Sign-In**</span></span> 

1. <span data-ttu-id="637a2-109">Nyissa meg az Azure AD bejelentkezési lapját.</span><span class="sxs-lookup"><span data-stu-id="637a2-109">Navigate to the Azure AD Sign-in page.</span></span>
1. <span data-ttu-id="637a2-110">A bejelentkezések szűrése felhasználó, időtartomány, alkalmazás, állapot, ügyfélalkalmazás stb. szerint.</span><span class="sxs-lookup"><span data-stu-id="637a2-110">Filter sign-ins by user, time range, application, status, client app, and so on.</span></span>
1. <span data-ttu-id="637a2-111">Jelöljön ki egy bejelentkezési eseményt, és tekintse meg a Feltételes hozzáférés lapot a kiértékelt házirendek megtekintéséhez.</span><span class="sxs-lookup"><span data-stu-id="637a2-111">Select a sign-in event and view the Conditional Access tab to see which policies were evaluated.</span></span>
1. <span data-ttu-id="637a2-112">Kattintson egy házirend sorra a házirend részleteinek megtekintéséhez és annak okának megtekintéséhez.</span><span class="sxs-lookup"><span data-stu-id="637a2-112">Click on the row of a policy to view the policy details and understand why it applied.</span></span>

<span data-ttu-id="637a2-113">**A feltételes hozzáférésre vonatkozó házirendek hibaelhárítási eszközei**</span><span class="sxs-lookup"><span data-stu-id="637a2-113">**Tools to troubleshoot a Conditional Access policy**</span></span>

- <span data-ttu-id="637a2-114">A csak jelentés módban a felhasználók befolyásolása nélkül értékelheti ki a házirendeket.</span><span class="sxs-lookup"><span data-stu-id="637a2-114">Report-only mode lets you evaluate a policy without impacting users.</span></span>
- <span data-ttu-id="637a2-115">A "mi van, ha" eszközzel szimulálhatja a bejelentkezési eseményeket, és megtekintheti, hogy mely házirendek érvényesek.</span><span class="sxs-lookup"><span data-stu-id="637a2-115">What-if tool lets you simulate sign-in events and see which policies apply.</span></span>
- <span data-ttu-id="637a2-116">A Betekintések és jelentéskészítési munkafüzet valós időben jeleníti meg az egyes házirendeket.</span><span class="sxs-lookup"><span data-stu-id="637a2-116">Insights and reporting workbook displays real-time impact of each policy.</span></span>

<span data-ttu-id="637a2-117">**Alaptervvédelmi házirendek**</span><span class="sxs-lookup"><span data-stu-id="637a2-117">**Baseline Protection Policies**</span></span>

<span data-ttu-id="637a2-118">Az Alaptervvédelmi házirendek elavultak.</span><span class="sxs-lookup"><span data-stu-id="637a2-118">Baseline Protection policies have been deprecated.</span></span> <span data-ttu-id="637a2-119">A továbbiakban nem érvényesíti őket a rendszer, és hamarosan el is távolítjuk őket az Azure Portalról.</span><span class="sxs-lookup"><span data-stu-id="637a2-119">They are no longer being enforced and will soon be removed from Azure portal.</span></span> <span data-ttu-id="637a2-120">Azt javasoljuk, hogy [engedélyezi a biztonsági alapértelmezett beállításokat.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)</span><span class="sxs-lookup"><span data-stu-id="637a2-120">We recommend enabling [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span>

<span data-ttu-id="637a2-121">A feltételes hozzáféréssel kapcsolatos további információkért lásd:</span><span class="sxs-lookup"><span data-stu-id="637a2-121">For more information on Conditional Access see:</span></span>

<span data-ttu-id="637a2-122">[Gyakorlati tanácsok az Azure Active Directory feltételes hozzáféréshez](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Feltételek a feltételes hozzáférésben](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Vezérlők a feltételes hozzáférésben](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Helyek a feltételes hozzáférésben](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span><span class="sxs-lookup"><span data-stu-id="637a2-122">[Best practices for conditional access in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Controls in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls) 
[Locations in Conditional Access ](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span></span>
