---
title: Példa az Office 365-nek az adathalászat elleni védelemre vonatkozó Microsoft Defenderre
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694036"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a><span data-ttu-id="2f9d0-102">Példa az Office 365-nek az adathalászat elleni védelemre vonatkozó Microsoft Defenderre</span><span class="sxs-lookup"><span data-stu-id="2f9d0-102">Example Microsoft Defender for Office 365 anti-phishing policy</span></span>

<span data-ttu-id="2f9d0-103">Ezek a beállítások engedélyezik a Domain and CEO (Tartomány és *igazgató) házirendet.*</span><span class="sxs-lookup"><span data-stu-id="2f9d0-103">These settings enable a policy called *Domain and CEO*.</span></span> <span data-ttu-id="2f9d0-104">Ez a házirend biztosítja a felhasználók és a tartományok védelmét a megszemélyesítés ellen, majd a tartományon belüli felhasználóktól kapott összes e-mailre alkalmazza a házirendet.</span><span class="sxs-lookup"><span data-stu-id="2f9d0-104">This policy provides both user and domain protection from impersonation and then applies the policy to all email received by users within the domain.</span></span> <span data-ttu-id="2f9d0-105">Először adja hozzá az alábbi adatokat a házirend létrehozásához:</span><span class="sxs-lookup"><span data-stu-id="2f9d0-105">First, add the following information to create the policy:</span></span>

- <span data-ttu-id="2f9d0-106">**Név:** Domain and CEO **Description**: Ensures that the CEO and your domain are not impersonated.</span><span class="sxs-lookup"><span data-stu-id="2f9d0-106">**Name**: Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.</span></span>
  <span data-ttu-id="2f9d0-107">**Alkalmazva:** Jelölje **ki a címzett tartományát.**</span><span class="sxs-lookup"><span data-stu-id="2f9d0-107">**Applied to**: Select **The recipient domain is**.</span></span> <span data-ttu-id="2f9d0-108">A **Válasszon, majd válasszon** egy tartományt a Beállítások csoportban. </span><span class="sxs-lookup"><span data-stu-id="2f9d0-108">Under **Any of these**, select **Choose**, and then select a domain.</span></span> <span data-ttu-id="2f9d0-109">Válassza **a + Hozzáadás gombot.**</span><span class="sxs-lookup"><span data-stu-id="2f9d0-109">Select **+ Add**.</span></span> <span data-ttu-id="2f9d0-110">Jelölje be a listában a tartomány neve melletti jelölőnégyzetet (például *contoso.com),* majd válassza az **Add (Hozzáadás) lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="2f9d0-110">Select the check box next to the name of the domain in the list (for example, *contoso.com*), and then select **Add**.</span></span> <span data-ttu-id="2f9d0-111">Válassza **a Kész gombot.**</span><span class="sxs-lookup"><span data-stu-id="2f9d0-111">Select **Done**.</span></span>
- <span data-ttu-id="2f9d0-112">A házirend létrehozása után a következő beállításokkal finomhangolhatja a házirendet:</span><span class="sxs-lookup"><span data-stu-id="2f9d0-112">After the policy is created, you can fine-tune the policy by using the following options:</span></span>
  - <span data-ttu-id="2f9d0-113">**Felhasználók hozzáadása védelemhez:** Ebben a példában adja meg legalább az igazgató e-mail-címét.</span><span class="sxs-lookup"><span data-stu-id="2f9d0-113">**Add users to protect:** For this example, add the CEO's email address, at a minimum.</span></span>
  - <span data-ttu-id="2f9d0-114">**Tartományok hozzáadása védelemhez:** Vegye fel azt a szervezeti tartományt, amely tartalmazza az ügyvezető igazgató irodáját.</span><span class="sxs-lookup"><span data-stu-id="2f9d0-114">**Add domains to protect**: Add the organizational domain that includes the office of the CEO.</span></span>
  - <span data-ttu-id="2f9d0-115">**Válassza ki a** műveleteket: Ha egy megszemélyesített felhasználó küldi az e-mailt, válassza az Üzenet átirányítása másik e-mail címre **lehetőséget,** majd adja meg a biztonsági rendszergazda *e-mail-címét*(például securityadmin@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="2f9d0-115">**Choose actions**: For **If email is sent by an impersonated user**, select **Redirect message to another email address**, and then enter the email address of the security administrator (for example, *securityadmin@contoso.com*).</span></span> <span data-ttu-id="2f9d0-116">Ha **megszemélyesített** tartomány küldi az e-maileket, válassza az üzenet **karanténba való kijelölését.**</span><span class="sxs-lookup"><span data-stu-id="2f9d0-116">For **If email is sent by an impersonated domain**, select **Quarantine the message**.</span></span>
  - <span data-ttu-id="2f9d0-117">**Postaláda-intelligencia:** Ez a beállítás alapértelmezés szerint be van jelölve új adathalászati házirend létrehozásakor.</span><span class="sxs-lookup"><span data-stu-id="2f9d0-117">**Mailbox intelligence**: By default, this option is selected when you create a new anti-phishing policy.</span></span> <span data-ttu-id="2f9d0-118">A legjobb eredmény érdekében hagyja **be** ezt a beállítást.</span><span class="sxs-lookup"><span data-stu-id="2f9d0-118">Leave this setting **On** for best results.</span></span>
  - <span data-ttu-id="2f9d0-119">**Megbízható feladók és tartományok hozzáadása:** Ebben a példában ne definiálja a felülbírálásokat.</span><span class="sxs-lookup"><span data-stu-id="2f9d0-119">**Add trusted senders and domains:** For this example, don't define any overrides.</span></span>
- <span data-ttu-id="2f9d0-120">Miután átnézte a beállításokat,  válassza a Házirend létrehozása vagy **a Mentés** lehetőséget a megfelelő módon.</span><span class="sxs-lookup"><span data-stu-id="2f9d0-120">Once you've reviewed your settings, select **Create this policy** or **Save**, as appropriate.</span></span>

<span data-ttu-id="2f9d0-121">További információt az adathalászat elleni házirendek [a Microsoft 365-ben.](https://go.microsoft.com/fwlink/?linkid=2092235)</span><span class="sxs-lookup"><span data-stu-id="2f9d0-121">To learn more, see [Anti-phishing policies in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span></span>
