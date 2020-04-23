---
title: Nem várt többtényezős hitelesítés
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ''
ms.custom:
- "1300007"
- "4372"
ms.openlocfilehash: a664bd709062ec1335ebcf1f9adddc8aef917ac1
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766603"
---
# <a name="unexpected-multi-factor-authentication"></a>Nem várt többtényezős hitelesítés

Ha a bérlői fiókját a 2019. október 21. után hozták létre, és Önt váratlanul többtényezős hitelesítésre kérik, akkor a bérlői fiókban valószínűleg engedélyezték az [alapértelmezett biztonsági beállításokat](https://aka.ms/securitydefaults). 

Az alapértelmezett biztonsági beállítások kezelése:

1. Jelentkezzen be a [felügyeleti központba](https://go.microsoft.com/fwlink/p/?linkid=834822) a globális rendszergazdai hitelesítő adataival.

2. Lépjen az [Azure Active Directory – Tulajdonságok](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties) lapra.

3. A lap alján válassza ki az **Alapértelmezett biztonsági beállítások kezelése** lehetőséget.

4. Válassza az **Igen** lehetőséget a biztonsági alapértékek engedélyezéséhez, és a **Nem** lehetőséget a biztonsági alapértékek letiltásához.
