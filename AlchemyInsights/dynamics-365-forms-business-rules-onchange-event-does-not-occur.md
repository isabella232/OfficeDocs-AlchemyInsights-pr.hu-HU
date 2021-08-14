---
title: Dynamics 365-űrlapok üzleti szabályai – Az üzleti szabály nem működik egy űrlapon
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 8425918950e1ef6c44f2866e6fa8987fe165536ae21e08ea6a1da880f761d512
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53947301"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Az OnChange esemény nem fordul elő, ha a mező programozással lett megváltoztatva

Az *OnChange* esemény nem fordul elő, ha a mező az attribútummal programozással *módosul.* [setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) metódus. Ha azt szeretné, hogy az *OnChange* esemény eseménykezelői futtassanak, miután beállította az értéket, a *formContext.data.entity* attribútum [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) metódusát kell használnia a kódban.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
