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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746855"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a><span data-ttu-id="08240-102">Példa az Office 365-nek az adathalászat elleni védelemre vonatkozó Microsoft Defenderre</span><span class="sxs-lookup"><span data-stu-id="08240-102">Example Microsoft Defender for Office 365 anti-phishing policy</span></span>

<span data-ttu-id="08240-103">Ezek a beállítások engedélyezik a Domain and CEO (Tartomány és *igazgató) nevű házirendet.*</span><span class="sxs-lookup"><span data-stu-id="08240-103">These settings enable a policy called *Domain and CEO*.</span></span> <span data-ttu-id="08240-104">Ez a házirend a felhasználók és a tartományok megszemélyesítése elleni védelmet is biztosítja, majd a tartományon belüli felhasználóktól kapott összes e-mailre alkalmazza a házirendet.</span><span class="sxs-lookup"><span data-stu-id="08240-104">This policy provides both user and domain protection from impersonation and then applies the policy to all email received by users within the domain.</span></span> <span data-ttu-id="08240-105">Először adja hozzá a következő információkat a házirend létrehozásához:</span><span class="sxs-lookup"><span data-stu-id="08240-105">First, add the following information to create the policy:</span></span>

- <span data-ttu-id="08240-106">**Név:** Domain and CEO Description : **Biztosítja,** hogy a CEO-t és a tartományt ne személyesítették meg.</span><span class="sxs-lookup"><span data-stu-id="08240-106">**Name**: Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.</span></span>
  <span data-ttu-id="08240-107">**Alkalmazva:** A **címzett tartományának kijelölése:**.</span><span class="sxs-lookup"><span data-stu-id="08240-107">**Applied to**: Select **The recipient domain is**.</span></span> <span data-ttu-id="08240-108">A **Válasszon egyet csoportban válassza** a Choose **(Választás)** lehetőséget, majd válasszon egy tartományt.</span><span class="sxs-lookup"><span data-stu-id="08240-108">Under **Any of these**, select **Choose**, and then select a domain.</span></span> <span data-ttu-id="08240-109">Válassza **a + Hozzáadás lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="08240-109">Select **+ Add**.</span></span> <span data-ttu-id="08240-110">Jelölje be a listában a tartomány neve melletti jelölőnégyzetet (például contoso.com *),* majd válassza a **Hozzáadás lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="08240-110">Select the check box next to the name of the domain in the list (for example, *contoso.com*), and then select **Add**.</span></span> <span data-ttu-id="08240-111">Válassza a **Kész lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="08240-111">Select **Done**.</span></span>
- <span data-ttu-id="08240-112">A házirend létrehozása után az alábbi beállításokkal finomhangolhatja a házirendet:</span><span class="sxs-lookup"><span data-stu-id="08240-112">After the policy is created, you can fine-tune the policy by using the following options:</span></span>
  - <span data-ttu-id="08240-113">**Felhasználók hozzáadása védelemhez:** Ebben a példában vegye fel legalább az ügyvezető igazgató e-mail-címét.</span><span class="sxs-lookup"><span data-stu-id="08240-113">**Add users to protect:** For this example, add the CEO's email address, at a minimum.</span></span>
  - <span data-ttu-id="08240-114">**Védjen meg tartományokat:** Vegye fel azt a szervezeti tartományt, amely tartalmazza az ügyvezető igazgató irodáját.</span><span class="sxs-lookup"><span data-stu-id="08240-114">**Add domains to protect**: Add the organizational domain that includes the office of the CEO.</span></span>
  - <span data-ttu-id="08240-115">Műveletek **kiválasztása:** Ha egy megszemélyesített felhasználó küldött e-mailt, válassza az Üzenet átirányítása másik e-mail címre **lehetőséget,** majd adja meg a biztonsági rendszergazda *e-mail-címét (például securityadmin@contoso.com).*</span><span class="sxs-lookup"><span data-stu-id="08240-115">**Choose actions**: For **If email is sent by an impersonated user**, select **Redirect message to another email address**, and then enter the email address of the security administrator (for example, *securityadmin@contoso.com*).</span></span> <span data-ttu-id="08240-116">Ha **megszemélyesített** tartomány küldi az e-maileket, válassza az Üzenet **karanténba küldése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="08240-116">For **If email is sent by an impersonated domain**, select **Quarantine the message**.</span></span>
  - <span data-ttu-id="08240-117">Postaláda-intelligencia: Új adathalászat-házirend létrehozásakor ez a beállítás alapértelmezés szerint be van jelölve.</span><span class="sxs-lookup"><span data-stu-id="08240-117">**Mailbox intelligence**: By default, this option is selected when you create a new anti-phishing policy.</span></span> <span data-ttu-id="08240-118">A legjobb eredmény érdekében hagyja **be a** beállítást.</span><span class="sxs-lookup"><span data-stu-id="08240-118">Leave this setting **On** for best results.</span></span>
  - <span data-ttu-id="08240-119">**Megbízható feladók és tartományok hozzáadása:** Ebben a példában ne definiálja a felülbírálásokat.</span><span class="sxs-lookup"><span data-stu-id="08240-119">**Add trusted senders and domains:** For this example, don't define any overrides.</span></span>
- <span data-ttu-id="08240-120">A beállítások áttekintése után válassza  a Házirend létrehozása vagy a **Mentés** lehetőséget a megfelelő módon.</span><span class="sxs-lookup"><span data-stu-id="08240-120">Once you've reviewed your settings, select **Create this policy** or **Save**, as appropriate.</span></span>

<span data-ttu-id="08240-121">További információ: [Adathalászat elleni házirendek a Microsoft 365-ben.](https://go.microsoft.com/fwlink/?linkid=2092235)</span><span class="sxs-lookup"><span data-stu-id="08240-121">To learn more, see [Anti-phishing policies in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span></span>
