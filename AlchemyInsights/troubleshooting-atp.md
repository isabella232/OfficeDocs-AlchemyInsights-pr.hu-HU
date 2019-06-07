---
title: Office 365 speciális veszély védelmi hibaelhárítás
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: b4358fb55a1145833510c6063b520d822f2d1eaf
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765141"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a><span data-ttu-id="de156-102">Office 365 speciális veszély védelmi hibaelhárítás</span><span class="sxs-lookup"><span data-stu-id="de156-102">Troubleshooting Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="de156-103">Figyelje az Üzenetkézbesítés késleltetése?</span><span class="sxs-lookup"><span data-stu-id="de156-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="de156-104">A biztonságos mellékletek ATP házirend a [Dinamikus kiszállítás](https://docs.microsoft.com/office365/securitycompliance/dynamic-delivery-and-previewing) beállítást használják.</span><span class="sxs-lookup"><span data-stu-id="de156-104">Use the [Dynamic Delivery](https://docs.microsoft.com/office365/securitycompliance/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="de156-105">Ez segít, miközben védi a címzettek rosszindulatú fájlokat az üzenet késedelmek elkerülése.</span><span class="sxs-lookup"><span data-stu-id="de156-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="de156-106">Ennek a hamis pozitív vagy hamis negatív jelentése a Microsoftnak?</span><span class="sxs-lookup"><span data-stu-id="de156-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="de156-107">E [hivatkozás](https://www.microsoft.com/wdsi/filesubmission/) segítségével elemzés fájlok elküldése.</span><span class="sxs-lookup"><span data-stu-id="de156-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="de156-108">Tudta, hogy engedélyezze a belső e-mail küldése a szervezeten belüli címzettekre közötti biztonságos kapcsolatok védelme?</span><span class="sxs-lookup"><span data-stu-id="de156-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="de156-109">Kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="de156-109">Follow these steps:</span></span>

  1. <span data-ttu-id="de156-110">Ugrás a [https://protection.office.com](https://protection.office.com) és a globális rendszergazdai vagy biztonsági rendszergazdai fiókkal jelentkezzen.</span><span class="sxs-lookup"><span data-stu-id="de156-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="de156-111">A **fenyegetés kezelés**alatt a bal oldali ablaktáblában, válassza a **házirend** \> **Biztonságos kapcsolatokat**.</span><span class="sxs-lookup"><span data-stu-id="de156-111">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="de156-112">A **házirendek, amelyek az egész szervezetre érvényes** szakaszban jelölje ki a házirendet, és kattintson a **Szerkesztés**gombra.</span><span class="sxs-lookup"><span data-stu-id="de156-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="de156-113">A **Beállítások**lehetővé teszik **a szervezeten belül elküldött üzenetek biztonságos hivatkozásokat alkalmaz**.</span><span class="sxs-lookup"><span data-stu-id="de156-113">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
