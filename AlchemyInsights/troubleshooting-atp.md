---
title: A Microsoft Defender Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 91d73853d3ea67d6c6954fffb32dd1428e3d9976
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545270"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="b784d-102">A Microsoft Defender Office 365</span><span class="sxs-lookup"><span data-stu-id="b784d-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="b784d-103">**Késik az üzenetek kézbesítése?**</span><span class="sxs-lookup"><span data-stu-id="b784d-103">**Do you notice delays in message delivery?**</span></span> <span data-ttu-id="b784d-104">A Microsoft Defender [Dinamikus kézbesítés](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) funkcióját használva Office 365 Széf mellékletek házirendjét.</span><span class="sxs-lookup"><span data-stu-id="b784d-104">Use the [Dynamic Delivery](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your Microsoft Defender for Office 365 Safe Attachments policy.</span></span> <span data-ttu-id="b784d-105">Ezzel megelőzheti az üzenetek késését, miközben védelmet nyújt a címzetteknek a kártékony fájloktól.</span><span class="sxs-lookup"><span data-stu-id="b784d-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="b784d-106">**Szeretne hamis pozitív vagy hamis negatív értékeket jelenteni a Microsoftnak?**</span><span class="sxs-lookup"><span data-stu-id="b784d-106">**Do you want to report false positives or false negatives to Microsoft?**</span></span> <span data-ttu-id="b784d-107">Használja [a Beküldéskezelőt.](https://protection.office.com/reportsubmission)</span><span class="sxs-lookup"><span data-stu-id="b784d-107">Use [Submissions Explorer](https://protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="b784d-108">-\*\* Tudta, hogy engedélyezheti a Széf hivatkozások elleni védelmet a szervezeten belüli címzettek között küldött belső e-mailekben?\*\* Kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="b784d-108">-\*\* Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?\*\* Follow these steps:</span></span>

  1. <span data-ttu-id="b784d-109">Jelentkezzen be globális rendszergazdai vagy [https://protection.office.com](https://protection.office.com) biztonsági rendszergazdai fiókkal.</span><span class="sxs-lookup"><span data-stu-id="b784d-109">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="b784d-110">A bal oldali navigációs ablakban a **Veszélyforrások kezelése** alatt válassza **a Házirendek** és \> **Széf lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="b784d-110">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="b784d-111">A teljes **szervezetre vonatkozó** házirendek szakaszban jelölje ki a házirendet, és kattintson a Szerkesztés **gombra.**</span><span class="sxs-lookup"><span data-stu-id="b784d-111">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="b784d-112">A **Gépház** alatt engedélyezze a Biztonságos hivatkozások alkalmazása a szervezeten belül **küldött üzenetekre beállítását.**</span><span class="sxs-lookup"><span data-stu-id="b784d-112">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
