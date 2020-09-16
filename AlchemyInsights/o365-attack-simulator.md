---
title: 2681-os támadás szimulátor a Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: dec96238c8438dcf9df176e3e3f20bd8a985b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47759221"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="d875f-102">Támadási szimulátor a Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="d875f-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="d875f-103">Hiányzik a támadási szimulátor?</span><span class="sxs-lookup"><span data-stu-id="d875f-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="d875f-104">A támadási szimulátorhoz az **office 365 Advanced Threat Protection Plan 2 (ATP-terv 2)** vagy az **Office 365 nagyvállalati E5**csomag szükséges.</span><span class="sxs-lookup"><span data-stu-id="d875f-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="d875f-105">A támadás-szimulátor **nem** része az Office 365 Advanced Threat Protection Plan 1 (ATP-terv 1), az Office 365 Enterprise E3 csomag vagy bármely Microsoft 365-alkalmazás vállalati verziós előfizetésnek.</span><span class="sxs-lookup"><span data-stu-id="d875f-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="d875f-106">A szimulált támadások elindításához használt fiók globális rendszergazdai vagy biztonsági rendszergazdai engedélyekkel és többtényezős hitelesítéssel (MFA) szükséges.</span><span class="sxs-lookup"><span data-stu-id="d875f-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="d875f-107">A támadási szimulátor követelményeiről a következő [témakörben](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)olvashat bővebben.</span><span class="sxs-lookup"><span data-stu-id="d875f-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="d875f-108">Fontos tudnivalók a **brute force jelszó** -támadási szimulációról:</span><span class="sxs-lookup"><span data-stu-id="d875f-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="d875f-109">Ha a célcella engedélyezve van, és a jelszó helyes volt, a fiók nem fog megjelenni a kiegyezésként (a második hitelesítési tényező hiányos lesz).</span><span class="sxs-lookup"><span data-stu-id="d875f-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="d875f-110">A jelszó-fájl nem lehet nagyobb 10 MB-nál.</span><span class="sxs-lookup"><span data-stu-id="d875f-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="d875f-111">Használjon soronként egy jelszót, és vegyen fel egy üres vonalat (kocsivissza) a lista utolsó jelszava után.</span><span class="sxs-lookup"><span data-stu-id="d875f-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="d875f-112">Fontos tudni, hogy a **célzott adathalászat** -szimulációk:</span><span class="sxs-lookup"><span data-stu-id="d875f-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="d875f-113">A terv szerint nem tud egyéni értéket biztosítani az **adathalászati bejelentkezési kiszolgáló URL-címéhez**.</span><span class="sxs-lookup"><span data-stu-id="d875f-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="d875f-114">Ha a címzettek [engedélyezik a jelentéskészítő üzenetben](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) az üzenet adathalászatként való jelentését, előfordulhat, hogy nem kap értesítést az üzenetről (mert szimulált támadás).</span><span class="sxs-lookup"><span data-stu-id="d875f-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="d875f-115">Jelentések: a szimulált támadás befejeződése után a **támadás részletei** hivatkozásra kattintva megtekintheti a jelentést.</span><span class="sxs-lookup"><span data-stu-id="d875f-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="d875f-116">A támadási szimulátorban a következő témakörben talál részletes útmutatást és új funkciókat: a [támadás szimulátor a Microsoft 365-ban](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="d875f-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
