---
title: Naplók és jelentéskészítés
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004331"
- "7727"
ms.openlocfilehash: 7349efb02f8d6ac5d73f6d6cd06eef6308ffe9be
ms.sourcegitcommit: 117c64e1fbcb5eec04f94eadad71423b974e7b14
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/27/2021
ms.locfileid: "50036014"
---
# <a name="logs-and-reporting"></a><span data-ttu-id="84799-102">Naplók és jelentéskészítés</span><span class="sxs-lookup"><span data-stu-id="84799-102">Logs and Reporting</span></span>

<span data-ttu-id="84799-103">[Az Azure Active Directory – gyakori](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) kérdések az Azure Active Directory (Azure AD) jelentéskészítéssel kapcsolatos gyakori kérdéseire ad választ.</span><span class="sxs-lookup"><span data-stu-id="84799-103">[Azure Active Directory reporting FAQ](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) answers frequently asked questions about Azure Active Directory (Azure AD) reporting.</span></span> <span data-ttu-id="84799-104">További információt az [Azure Active Directory jelentéskészítési szolgáltatásában.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports)</span><span class="sxs-lookup"><span data-stu-id="84799-104">For more information, see [Azure Active Directory reporting](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).</span></span>

<span data-ttu-id="84799-105">**A naplózással kapcsolatos hibák elhárítása**</span><span class="sxs-lookup"><span data-stu-id="84799-105">**Troubleshooting issues with Audit**</span></span>

1. <span data-ttu-id="84799-106">Ha bizonyos naplózási tevékenységeket nem lát, és a hiányzó tevékenység szerepel ezen a [listán,](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities)kérjük, írjon egy támogatási jegyet.</span><span class="sxs-lookup"><span data-stu-id="84799-106">If you are having issues seeing some audit activities and the missing Activity is in this [list](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities), please file a support ticket.</span></span>
2. <span data-ttu-id="84799-107">Ha problémákat jelentkezik a naplók megtekintése a bérlői webhelyen, kérjük, írjon be egy támogatási jegyet.</span><span class="sxs-lookup"><span data-stu-id="84799-107">If you are having issues seeing any Audit logs in your tenant, please file a support ticket.</span></span>
3. <span data-ttu-id="84799-108">Ha a naplózási tevékenységek nem adatokat tartalmaznak [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) azonnal az Azure Portal webhelyen, tekintse meg a késéssel kapcsolatos információkat, és ha a késés meghaladja a dokumentált késést, egy támogatási jegyet nyújt be.</span><span class="sxs-lookup"><span data-stu-id="84799-108">If your audit activities are not showing up immediately in the Azure Portal, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. [<span data-ttu-id="84799-109">Azure AD-tevékenységnaplók megőrzés</span><span class="sxs-lookup"><span data-stu-id="84799-109">Azure AD Activity Logs Retention</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. <span data-ttu-id="84799-110">Ha nem látja a kijelölt dátumtartomány összes naplóját, az Azure Portalról akár 250 000 sort is letölthet (a legutóbbi szerint rendezve).</span><span class="sxs-lookup"><span data-stu-id="84799-110">If you don't see all the audit for the date range you selected, you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="84799-111">További információ: [Naplózási tevékenységek letöltése.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report)</span><span class="sxs-lookup"><span data-stu-id="84799-111">For more information, see [Audit activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span></span>

<span data-ttu-id="84799-112">**Bejelentkezési problémák elhárítása**</span><span class="sxs-lookup"><span data-stu-id="84799-112">**Troubleshooting issues with Sign-ins**</span></span>

1. <span data-ttu-id="84799-113">Az elmúlt 30 nap adatait csak akkor láthatja, ha a bérlőjéhez Azure AD Premium (P1 vagy P2) licenccel rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="84799-113">You can only see the last 30 days of data if you have an Azure AD Premium (P1 or P2) license for your tenant.</span></span>
2. <span data-ttu-id="84799-114">A bejelentkezések csak Azure AD Prémium bérlői fiók esetén érhetők el.</span><span class="sxs-lookup"><span data-stu-id="84799-114">Sign-ins are available only for Azure AD Premium tenants.</span></span> <span data-ttu-id="84799-115">Az ingyenes és az alapszintű licenccel rendelkező bérlők nem érhetők el.</span><span class="sxs-lookup"><span data-stu-id="84799-115">It's not available for Free or Basic licensed tenants.</span></span>
3. <span data-ttu-id="84799-116">Ha a bérlő rendelkezik prémium P1 licenccel, és Ön nem látja [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) a bejelentkezéseket, tekintse meg a késéssel kapcsolatos információkat, és írjon egy támogatási jegyet, ha a késés meghaladja a dokumentált késést.</span><span class="sxs-lookup"><span data-stu-id="84799-116">If your tenant has a Premium P1 license and you can't see the sign-ins, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. <span data-ttu-id="84799-117">Ha nem látja a kijelölt dátumtartomány összes bejelentkezését, ne feledje, hogy az Azure Portalról akár 250 000 sort is letölthet (a legutóbbiak szerint rendezve).</span><span class="sxs-lookup"><span data-stu-id="84799-117">If you don't see all the sign-ins for the date range you selected, note that you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="84799-118">További információ: Bejelentkezési tevékenységek [letöltése.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities)</span><span class="sxs-lookup"><span data-stu-id="84799-118">For more information, see [Sign-ins activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span></span>

<span data-ttu-id="84799-119">**Biztonsági jelentések hibaelhárítása (A kockázatnak megjelölt felhasználók, kockázatos bejelentkezés)**</span><span class="sxs-lookup"><span data-stu-id="84799-119">**Troubleshoot Security Reports (Users Flagged at Risk, Risky Sign-In)**</span></span>

1. [<span data-ttu-id="84799-120">A kockázatok biztonsági jelentésére megjelölt felhasználók</span><span class="sxs-lookup"><span data-stu-id="84799-120">Users flagged for risk security report</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [<span data-ttu-id="84799-121">Kockázatos bejelentkezési jelentések az Azure Active Directory portálon</span><span class="sxs-lookup"><span data-stu-id="84799-121">Risky sign-ins report in the Azure Active Directory portal</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [<span data-ttu-id="84799-122">Azure Active Directory –kockázatesemények</span><span class="sxs-lookup"><span data-stu-id="84799-122">Azure Active Directory risk events</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
