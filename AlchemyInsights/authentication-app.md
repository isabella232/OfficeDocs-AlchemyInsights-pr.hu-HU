---
title: Authentication app
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405063"
---
# <a name="authentication-app"></a><span data-ttu-id="db815-102">Authentication app</span><span class="sxs-lookup"><span data-stu-id="db815-102">Authentication app</span></span>

<span data-ttu-id="db815-103">Ha Ön globális rendszergazda, a Bejelentkezés diagnosztika segítségével gyorsan kiderítheti, hogy mi történt, vagy diagnosztizálhatja a felhasználói bejelentkezéssel [kapcsolatos problémákat.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="db815-103">If you are a Global Admin, you can quickly find out what happened or diagnose problems related to user-sign in by using the [Sign-in Diagnostics](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>

1. <span data-ttu-id="db815-104">Indítsa el a diagnosztikát a "[Diagnosztikai indítása" gombra](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)kattintva.</span><span class="sxs-lookup"><span data-stu-id="db815-104">Start the diagnostics by clicking "[Launch Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" button.</span></span> 
1. <span data-ttu-id="db815-105">Keresse meg az elemezni szükséges eseményt a felhasználóval, alkalmazással, a bejelentkezés időpontjával, a kérelem azonosítójával vagy a korrelációs azonosítóval kapcsolatos részletek megadásával.</span><span class="sxs-lookup"><span data-stu-id="db815-105">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="db815-106">Tekintse át a diagnosztikai eredményeket, és nézze meg, hogy mi történt, és milyen műveleteket lehet tenni a módosításokhoz, ha szükség van módosításokra.</span><span class="sxs-lookup"><span data-stu-id="db815-106">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="db815-107">**Ellenőrizze a megfelelő esetet:**</span><span class="sxs-lookup"><span data-stu-id="db815-107">**Check the scenario that is applicable:**</span></span>

1. <span data-ttu-id="db815-108">Ha egy felhasználó nem kap leküldéses értesítést a Microsoft Authenticator appban, ellenőrizze, hogy nem jelennek-e meg az MFA által letiltott felhasználók között a Felhasználók blokkolása és letiltásának feloldása csoportban leírtak [szerint.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="db815-108">If a user is not getting a push notification in the Microsoft Authenticator app, verify they are not shown under the MFA blocked users as described in [Block and unblock users](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
1. <span data-ttu-id="db815-109">Ha a felhasználó nincs letiltva több hitelesítésre, de nem kap leküldéses értesítést, megnyithatja a Microsoft Authenticator appot, amely lekérte a függőben lévő jóváhagyási kérelmeket.</span><span class="sxs-lookup"><span data-stu-id="db815-109">If the user is not blocked for MFA but does not receive a push notification, they can open the Microsoft Authenticator app, which will pull the pending approval requests.</span></span>
1. <span data-ttu-id="db815-110">Másik bejelentkezési módszerként a felhasználó a Bejelentkezés más módon elemre is kattinthat, és kiválaszthatja a mobilappom ellenőrző kódját.</span><span class="sxs-lookup"><span data-stu-id="db815-110">As an alternative sign-in method, the user can also click on Sign in another way and choose use a verification code from my mobile app.</span></span>
1. <span data-ttu-id="db815-111">Sok felhasználó csak a Microsoft Authenticator appot érhetők el.</span><span class="sxs-lookup"><span data-stu-id="db815-111">The Microsoft Authenticator App is the only available method for many users.</span></span> <span data-ttu-id="db815-112">[További információ a biztonsági](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)alapértelmezett beállításokról , az [Authenticator app](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) gyakori kérdéseinek gyakori kérdéseiről és a megoldásukról.</span><span class="sxs-lookup"><span data-stu-id="db815-112">[Learn more about security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), check [Authenticator App FAQ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) for commonly asked questions and how to resolve them.</span></span>
 
<span data-ttu-id="db815-113">**Ajánlott videók**</span><span class="sxs-lookup"><span data-stu-id="db815-113">**Recommended Videos**</span></span>

<span data-ttu-id="db815-114">[Az Authenticator app beállítása új telefonon (2min).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)</span><span class="sxs-lookup"><span data-stu-id="db815-114">[How to set up Authenticator App on a new phone (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span></span>
