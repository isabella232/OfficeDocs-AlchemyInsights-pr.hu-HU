---
title: Az SMTP-hitelesítéssel kapcsolatos problémák megoldása
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826417"
---
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="7491c-102">Az SMTP-hitelesítéssel kapcsolatos problémák megoldása</span><span class="sxs-lookup"><span data-stu-id="7491c-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="7491c-103">Ha 5.7.57-es vagy 5.7.3-as kódú hiba történik, amikor SMTP-alapú e-mailt próbál küldeni, és hitelesítést szeretne végezni egy ügyféllel vagy alkalmazással, érdemes ellenőriznie néhány dolgot:</span><span class="sxs-lookup"><span data-stu-id="7491c-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="7491c-104">Előfordulhat, hogy a hitelesített SMTP-küldés le van tiltva a bérlőben vagy a használni próbált postaládában (mindkét beállítást ellenőrizze).</span><span class="sxs-lookup"><span data-stu-id="7491c-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="7491c-105">További információt a [Hitelesített ügyfél általi SMTP-küldés engedélyezése vagy letiltása](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission) című cikkben olvashat.</span><span class="sxs-lookup"><span data-stu-id="7491c-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="7491c-106">Ellenőrizze, hogy engedélyezve vannak-e az [Azure alapértelmezett biztonsági beállításai](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) a bérlőjéhez. Ha engedélyezve vannak, az alapszintű hitelesítéssel (más néven régi hitelesítéssel, felhasználónév és jelszó használatával) történő SMTP-hitelesítés nem fog sikerülni.</span><span class="sxs-lookup"><span data-stu-id="7491c-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>
