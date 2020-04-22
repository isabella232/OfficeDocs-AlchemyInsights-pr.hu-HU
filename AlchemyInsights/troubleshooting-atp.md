---
title: Az Office 365 komplex veszélyforrások elleni védelem hibáinak elhárítása
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: c90c8e9cb23cba93883cc1148fcbca77c9e92408
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732404"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a><span data-ttu-id="e3235-102">Az Office 365 komplex veszélyforrások elleni védelem hibáinak elhárítása</span><span class="sxs-lookup"><span data-stu-id="e3235-102">Troubleshooting Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="e3235-103">Késést észlel az üzenetek kézbesítésében?</span><span class="sxs-lookup"><span data-stu-id="e3235-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="e3235-104">Használja a [dinamikus kézbesítés](https://docs.microsoft.com/office365/securitycompliance/dynamic-delivery-and-previewing) i.use the Dynamic Delivery option in your ATP Safe Attachments policy.</span><span class="sxs-lookup"><span data-stu-id="e3235-104">Use the [Dynamic Delivery](https://docs.microsoft.com/office365/securitycompliance/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="e3235-105">Ez segít elkerülni az üzenetek késleltetését, miközben megvédi a címzetteket a rosszindulatú fájloktól.</span><span class="sxs-lookup"><span data-stu-id="e3235-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="e3235-106">Hamis pozitív vagy hamis negatív értékeket szeretne jelenteni a Microsoftnak?</span><span class="sxs-lookup"><span data-stu-id="e3235-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="e3235-107">Ezen a [hivatkozáson](https://www.microsoft.com/wdsi/filesubmission/) fájlokat küldhet elemzésre.</span><span class="sxs-lookup"><span data-stu-id="e3235-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="e3235-108">Tudta, hogy engedélyezheti a biztonságos hivatkozások védelmét a szervezeten belüli címzettek között küldött belső e-mailek számára?</span><span class="sxs-lookup"><span data-stu-id="e3235-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="e3235-109">Hajtsa végre az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="e3235-109">Follow these steps:</span></span>

  1. <span data-ttu-id="e3235-110">Lépjen [https://protection.office.com](https://protection.office.com) a globális rendszergazdai vagy biztonsági rendszergazdai fiókkal, és jelentkezzen be.</span><span class="sxs-lookup"><span data-stu-id="e3235-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="e3235-111">A **fenyegetéskezelés**csoport bal oldali navigációs ablakában válassza a **Házirendbiztonságos** \> **hivatkozások lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="e3235-111">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="e3235-112">A **teljes szervezetre vonatkozó házirendek** csoportban jelölje ki a házirendet, és kattintson a **Szerkesztés gombra.**</span><span class="sxs-lookup"><span data-stu-id="e3235-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="e3235-113">A **Beállítások csoportban**engedélyezze **a Biztonságos hivatkozások alkalmazása a szervezeten belül küldött üzenetekre.**</span><span class="sxs-lookup"><span data-stu-id="e3235-113">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
