---
title: Felhasználói bejelentkezési hibák
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7790"
- "9004355"
ms.openlocfilehash: 05bd31cb4afecf1342e040eecd9e58cd38bd8d49
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900990"
---
# <a name="user-sign-in-errors"></a><span data-ttu-id="be136-102">Felhasználói bejelentkezési hibák</span><span class="sxs-lookup"><span data-stu-id="be136-102">User sign-in errors</span></span>

<span data-ttu-id="be136-103">**A bejelentkezés diagnosztikai problémáinak megoldása**</span><span class="sxs-lookup"><span data-stu-id="be136-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="be136-104">A felhasználói bejelentkezéssel kapcsolatos problémák okának vagy diagnosztizálásához végezze el az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="be136-104">To detect the cause or diagnose problems related to user sign-in, perform the following steps:</span></span>

1. <span data-ttu-id="be136-105">Indítsa el [a bejelentkezés diagnosztikai eszközét.](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="be136-105">Launch the [Sign-in Diagnostic](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
2. <span data-ttu-id="be136-106">Keresse meg az elemezni szükséges eseményt a felhasználóval, alkalmazással, a bejelentkezés időpontjával, a kérelem azonosítójával vagy a korrelációs azonosítóval kapcsolatos adatok megadásával.</span><span class="sxs-lookup"><span data-stu-id="be136-106">Find the event to analyze by entering the details you have about the user, application, time of sign in, request Id, or correlation Id.</span></span>
3. <span data-ttu-id="be136-107">Tekintse át a diagnosztikai eredményeket, amelyekben látható, hogy mi történt, és milyen műveleteket lehet tenni a módosítások végrehajtása érdekében, ha szükség van módosításokra.</span><span class="sxs-lookup"><span data-stu-id="be136-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="be136-108">**Az Azure Active Directory (Azure AD) biztonsági jogkivonat-szolgáltatásból (STS) visszaadott AADSTS-hibakódokkal kapcsolatos információkat keres?**</span><span class="sxs-lookup"><span data-stu-id="be136-108">**Looking for information about the AADSTS error codes that are returned from the Azure Active Directory (Azure AD) security token service (STS)?**</span></span> <span data-ttu-id="be136-109">Ebben [a cikkben](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) megtalálja az AADSTS hibaleírásokat, javításokat és néhány javasolt kerülő megoldást.</span><span class="sxs-lookup"><span data-stu-id="be136-109">Read [this article](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) to find AADSTS error descriptions, fixes, and some suggested workarounds</span></span>