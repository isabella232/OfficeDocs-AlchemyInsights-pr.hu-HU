---
title: Dynamics 365 Forms üzleti szabályok-üzleti szabály nem égetés űrlap
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 3cdd2175083e864b3bffc57a70bb6c6220843fad
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/15/2019
ms.locfileid: "37769341"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>A OnChange esemény nem következik be, ha a mező programozás útján módosul

A *OnChange* esemény nem fordul elő, ha a mező programozás útján, az *attribútum* használatával módosul. [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) metódus. Ha azt szeretné, hogy a *OnChange* esemény eseménykezelőit az érték beállítása után futtassuk, akkor a kódban a *formcontext. Data. entitás attribútumnak* a [fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) metódust kell használnia.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
