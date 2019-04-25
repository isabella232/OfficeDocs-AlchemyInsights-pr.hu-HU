---
title: Az Office 365 speciális veszély védelmi (ATP) kapcsolatos problémák elhárítása
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: dbdfe2ddcc4afd4477f66ffd060ddb7093af8fd6
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420306"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="29acf-102">Office 365 ATP problémáinak elhárítása</span><span class="sxs-lookup"><span data-stu-id="29acf-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="29acf-103">**Az e-mail üzenet kézbesítési értesítés késedelem**?</span><span class="sxs-lookup"><span data-stu-id="29acf-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="29acf-104">Próbálja meg használni a dinamikus kiszállítás beállítást az ATP biztonságos mellékletek házirendek.</span><span class="sxs-lookup"><span data-stu-id="29acf-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="29acf-105">E-mail üzenet kézbesítési késések így elkerülhető, miközben védi a címzettek a rosszindulatú fájlokat.</span><span class="sxs-lookup"><span data-stu-id="29acf-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="29acf-106">A **kívánt jelentés hamis pozitív vagy hamis negatív**?</span><span class="sxs-lookup"><span data-stu-id="29acf-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="29acf-107">E hivatkozás segítségével a fájl elemzéséhez nyújt:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="29acf-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="29acf-108">**Tudja, hogy engedélyezze a biztonságos kapcsolatok ATP védelmet a szervezet tagjai között küldött e-mail**?</span><span class="sxs-lookup"><span data-stu-id="29acf-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="29acf-109">Kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="29acf-109">Follow these steps:</span></span>
    1. <span data-ttu-id="29acf-110">Ugrás a https://protection.office.com, és jelentkezzen be.</span><span class="sxs-lookup"><span data-stu-id="29acf-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="29acf-111">Ugrás a **fenyegetés kezelése** > **politika** > **Biztonságos kapcsolatokat**.</span><span class="sxs-lookup"><span data-stu-id="29acf-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="29acf-112">**A megadott címzetteknek érvényes házirendek**szerkesztése vagy hozzáadása egy házirend.</span><span class="sxs-lookup"><span data-stu-id="29acf-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="29acf-113">Válassza ki **a szervezeten belül elküldött üzenetek biztonságos hivatkozásokat alkalmaz**.</span><span class="sxs-lookup"><span data-stu-id="29acf-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="29acf-114">A házirend mentése, és lehetővé teszi a módosítások a datacenter keresztül haladva körülbelül 30 percig.</span><span class="sxs-lookup"><span data-stu-id="29acf-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="29acf-115">További segítség az Ígérethez rendelkezésre álló mennyiség, olvassa el az [Office 365 speciális veszély védelmi](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="29acf-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).</span></span>