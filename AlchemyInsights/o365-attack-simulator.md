---
title: 2681 támadás Szimuláns hivatalban 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 07d7622c00074f7bd0d567185824db448f1eeef3
ms.sourcegitcommit: 7232b48bcd8bb9867d52a2f055a46ce76a58b8da
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "37305334"
---
# <a name="attack-simulator-in-office-365"></a><span data-ttu-id="51448-102">Támadás Szimuláns hivatalban 365</span><span class="sxs-lookup"><span data-stu-id="51448-102">Attack Simulator in Office 365</span></span>

- <span data-ttu-id="51448-103">Van ön hiányzó támadás Szimuláns?</span><span class="sxs-lookup"><span data-stu-id="51448-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="51448-104">Támadás szimulátor megkövetel **hivatal 365 haladó fenyeget védelem tervez 2 (ATP tervez 2)** vagy **Hivatal 365 vállalat E5**.</span><span class="sxs-lookup"><span data-stu-id="51448-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="51448-105">Támadás Szimuláns van **nem** tartalmazott-ban Hivatal 365 haladó fenyeget védelem tervez 1 (ATP tervez 1), Hivatal 365 vállalat E3, vagy akármi Hivatal 365 teendő előfizetések.</span><span class="sxs-lookup"><span data-stu-id="51448-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Office 365 Business subscriptions.</span></span>

- <span data-ttu-id="51448-106">A szimulált támadások elindításához használt fióknak globális rendszergazdai vagy biztonsági rendszergazdai engedélyekre és többtényezős hitelesítésre van szüksége (MFA).</span><span class="sxs-lookup"><span data-stu-id="51448-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="51448-107">A támadási követelményekkel kapcsolatos további tudnivalókért tanulmányozza ezt a [témakört](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span><span class="sxs-lookup"><span data-stu-id="51448-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span></span>

- <span data-ttu-id="51448-108">Fontos dolgok tudni **brute force jelszó** támadás szimuláció:</span><span class="sxs-lookup"><span data-stu-id="51448-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="51448-109">Ha a célfiókhoz engedélyezve van az MFA, és a jelszó helyesen lett kitalálható, a fiók nem jelenik meg veszélybe (a második hitelesítési tényező nem lesz teljes).</span><span class="sxs-lookup"><span data-stu-id="51448-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="51448-110">A jelszófájl nem lehet nagyobb 10 MB-nál.</span><span class="sxs-lookup"><span data-stu-id="51448-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="51448-111">Soronként egy jelszót használjon, és a lista utolsó jelszava után üres sort (kocsivissza) is használhat.</span><span class="sxs-lookup"><span data-stu-id="51448-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="51448-112">Fontos tudnivalók a **lándzsával kapcsolatos adathalászó** szimulációkhoz:</span><span class="sxs-lookup"><span data-stu-id="51448-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="51448-113">Tervezéssel nem biztosíthat egyéni értéket az **adathalász bejelentkezési kiszolgáló URL-címének**.</span><span class="sxs-lookup"><span data-stu-id="51448-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="51448-114">Ha a címzett engedélyezi a [jelentésüzenet bővítmény](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) számára az üzenet adathalászattal történő jelentésének engedélyezését, akkor előfordulhat, hogy nem kap figyelmeztetést az üzenethez (mivel ez egy szimulált támadás).</span><span class="sxs-lookup"><span data-stu-id="51448-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="51448-115">Jelentések: Miután befejeződött a szimulált támadás, a jelentés megtekintéséhez kattintson a **támadási adatok** gombra.</span><span class="sxs-lookup"><span data-stu-id="51448-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="51448-116">Részére részletes oktatás és új jellegét meghatározza-ban támadás Szimuláns, lát [támadás Szimuláns hivatalban 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="51448-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
