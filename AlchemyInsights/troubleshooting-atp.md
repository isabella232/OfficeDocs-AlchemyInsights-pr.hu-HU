---
title: Hibaelhárítás a Microsoft Defender for Office 365-ban
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
ms.openlocfilehash: 2c9543660056ebc02b0bd297f619f20fa6820093
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801445"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="06b42-102">Hibaelhárítás a Microsoft Defender for Office 365-ban</span><span class="sxs-lookup"><span data-stu-id="06b42-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="06b42-103">Tapasztal késedelmet az üzenet kézbesítésében?</span><span class="sxs-lookup"><span data-stu-id="06b42-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="06b42-104">Használja a [dinamikus kézbesítési](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) lehetőséget az ATP Safe mellékletek házirendjében.</span><span class="sxs-lookup"><span data-stu-id="06b42-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="06b42-105">Ez segít elkerülni az üzenetek késleltetését, miközben megvédi a címzetteket a kártékony fájlokból.</span><span class="sxs-lookup"><span data-stu-id="06b42-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="06b42-106">Hamis pozitív vagy hamis negatívokat szeretne jelenteni a Microsoftnak?</span><span class="sxs-lookup"><span data-stu-id="06b42-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="06b42-107">Ezzel a [hivatkozással](https://www.microsoft.com/wdsi/filesubmission/) elküldhet fájlokat az elemzéshez.</span><span class="sxs-lookup"><span data-stu-id="06b42-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="06b42-108">Tudta, hogy a szervezeten belüli címzettek által küldött belső e-mailek biztonsága érdekében engedélyezheti a biztonságos hivatkozások védelmét?</span><span class="sxs-lookup"><span data-stu-id="06b42-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="06b42-109">Hajtsa végre az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="06b42-109">Follow these steps:</span></span>

  1. <span data-ttu-id="06b42-110">Lépjen [https://protection.office.com](https://protection.office.com) egy globális rendszergazdai vagy biztonsági rendszergazdai fiókjával, és lépjen be.</span><span class="sxs-lookup"><span data-stu-id="06b42-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="06b42-111">A bal oldali navigációs ablakban a **fenyegetések kezelése** csoportban válassza a **házirend** - \> **megbízható hivatkozások** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="06b42-111">In the left navigation pane under **Threat management** , choose **Policy** \> **Safe Links** .</span></span>

  3. <span data-ttu-id="06b42-112">A teljes szervezet szakaszra vonatkozó **házirendekben** jelölje ki a házirendet, és kattintson a **Szerkesztés** gombra.</span><span class="sxs-lookup"><span data-stu-id="06b42-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit** .</span></span>

  4. <span data-ttu-id="06b42-113">A **Beállítások** csoportban engedélyezze **a biztonságos hivatkozások alkalmazása a szervezeten belül küldött üzenetekre** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="06b42-113">Under **Settings** , enable **Apply safe links to messages sent within the organization** .</span></span>
