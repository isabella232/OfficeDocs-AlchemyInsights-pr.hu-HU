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
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="5385e-102">A OnChange esemény nem következik be, ha a mező programozás útján módosul</span><span class="sxs-lookup"><span data-stu-id="5385e-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="5385e-103">A *OnChange* esemény nem fordul elő, ha a mező programozás útján, az *attribútum* használatával módosul. [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) metódus.</span><span class="sxs-lookup"><span data-stu-id="5385e-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="5385e-104">Ha azt szeretné, hogy a *OnChange* esemény eseménykezelőit az érték beállítása után futtassuk, akkor a kódban a *formcontext. Data. entitás attribútumnak* a [fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) metódust kell használnia.</span><span class="sxs-lookup"><span data-stu-id="5385e-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
