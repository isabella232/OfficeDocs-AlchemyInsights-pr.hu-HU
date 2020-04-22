---
title: 2681 Támadás szimulátor a Microsoft 365-ben
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 74bd2dd62b24aaf6c9d7b387ab1d97ddab31e902
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713468"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="70aaf-102">Támadás szimulátor a Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="70aaf-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="70aaf-103">Hiányzik támadás szimulátor?</span><span class="sxs-lookup"><span data-stu-id="70aaf-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="70aaf-104">A Támadásszimulátor használatához az **Office 365 Komplex veszélyforrások elleni védelem 2.** **Office 365 Enterprise E5**</span><span class="sxs-lookup"><span data-stu-id="70aaf-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="70aaf-105">Az Attack Simulator **nem** része az Office 365 Komplex veszélyforrások elleni védelem 1., 1.</span><span class="sxs-lookup"><span data-stu-id="70aaf-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="70aaf-106">A szimulált támadások indításához használt fiókhoz globális rendszergazdai vagy biztonsági rendszergazdai engedélyekés többtényezős hitelesítés (MFA) szükséges.</span><span class="sxs-lookup"><span data-stu-id="70aaf-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="70aaf-107">Az Attack Simulator követelményeiről a [jelen témakörben](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin)olvashat bővebben.</span><span class="sxs-lookup"><span data-stu-id="70aaf-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span></span>

- <span data-ttu-id="70aaf-108">Fontos tudnivalók a **Brute Force Password** támadásszimulációiról:</span><span class="sxs-lookup"><span data-stu-id="70aaf-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="70aaf-109">Ha a célfiókban engedélyezve van az MFA, és a jelszó helyesen lett kitalálva, a fiók nem jelenik meg feltörtként (a második hitelesítési tényező nem lesz teljes).</span><span class="sxs-lookup"><span data-stu-id="70aaf-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="70aaf-110">A jelszófájl nem lehet nagyobb 10 MB-nál.</span><span class="sxs-lookup"><span data-stu-id="70aaf-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="70aaf-111">Soronként egy jelszót használjon, és a lista utolsó jelszava után adjon meg egy üres sort (kocsivissza).</span><span class="sxs-lookup"><span data-stu-id="70aaf-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="70aaf-112">Fontos tudnivalók a **spear phishing** csatolásáról szimulációk:</span><span class="sxs-lookup"><span data-stu-id="70aaf-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="70aaf-113">Az **adathalászat-kiszolgáló URL-címéhez**nem adhat meg egyéni értéket.</span><span class="sxs-lookup"><span data-stu-id="70aaf-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="70aaf-114">Ha a címzett [a Jelentésüzenet engedélyezése bővítményt](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) használja az üzenet adathalászatként való jelentéséhez, előfordulhat, hogy nem kap értesítést az üzenetről (mivel ez egy szimulált támadás).</span><span class="sxs-lookup"><span data-stu-id="70aaf-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="70aaf-115">Jelentések: A szimulált támadás befejezése után a **támadás részletei** gombra kattintva megtekintheti a jelentést.</span><span class="sxs-lookup"><span data-stu-id="70aaf-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="70aaf-116">Az Attack Simulator részletes útmutatásait és új funkcióit a [Microsoft 365 Támadásszimulátor című témakörében találja.](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="70aaf-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
