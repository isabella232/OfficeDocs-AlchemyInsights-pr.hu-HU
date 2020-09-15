---
title: Az Office 365 Advanced Threat Protection – hibaelhárítás
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
ms.openlocfilehash: 5a13653ba08d8c6b822354ff70f6d276d31cd816
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658916"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a><span data-ttu-id="1e177-102">Az Office 365 Advanced Threat Protection – hibaelhárítás</span><span class="sxs-lookup"><span data-stu-id="1e177-102">Troubleshooting Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="1e177-103">Tapasztal késedelmet az üzenet kézbesítésében?</span><span class="sxs-lookup"><span data-stu-id="1e177-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="1e177-104">Használja a [dinamikus kézbesítési](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) lehetőséget az ATP Safe mellékletek házirendjében.</span><span class="sxs-lookup"><span data-stu-id="1e177-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="1e177-105">Ez segít elkerülni az üzenetek késleltetését, miközben megvédi a címzetteket a kártékony fájlokból.</span><span class="sxs-lookup"><span data-stu-id="1e177-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="1e177-106">Hamis pozitív vagy hamis negatívokat szeretne jelenteni a Microsoftnak?</span><span class="sxs-lookup"><span data-stu-id="1e177-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="1e177-107">Ezzel a [hivatkozással](https://www.microsoft.com/wdsi/filesubmission/) elküldhet fájlokat az elemzéshez.</span><span class="sxs-lookup"><span data-stu-id="1e177-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="1e177-108">Tudta, hogy a szervezeten belüli címzettek által küldött belső e-mailek biztonsága érdekében engedélyezheti a biztonságos hivatkozások védelmét?</span><span class="sxs-lookup"><span data-stu-id="1e177-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="1e177-109">Hajtsa végre az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="1e177-109">Follow these steps:</span></span>

  1. <span data-ttu-id="1e177-110">Lépjen [https://protection.office.com](https://protection.office.com) egy globális rendszergazdai vagy biztonsági rendszergazdai fiókjával, és lépjen be.</span><span class="sxs-lookup"><span data-stu-id="1e177-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="1e177-111">A bal oldali navigációs ablakban a **fenyegetések kezelése**csoportban válassza a **házirend** - \> **megbízható hivatkozások**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="1e177-111">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="1e177-112">A teljes szervezet szakaszra vonatkozó **házirendekben** jelölje ki a házirendet, és kattintson a **Szerkesztés**gombra.</span><span class="sxs-lookup"><span data-stu-id="1e177-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="1e177-113">A **Beállítások**csoportban engedélyezze **a biztonságos hivatkozások alkalmazása a szervezeten belül küldött üzenetekre**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="1e177-113">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
