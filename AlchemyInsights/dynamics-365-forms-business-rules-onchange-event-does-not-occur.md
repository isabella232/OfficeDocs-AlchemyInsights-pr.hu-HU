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
ms.openlocfilehash: cbdedd2c5fcf5517243e60e36d86479d6c3f7814
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/18/2019
ms.locfileid: "36529021"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="4c3f1-102">A OnChange esemény nem következik be, ha a mező programozás útján módosul</span><span class="sxs-lookup"><span data-stu-id="4c3f1-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="4c3f1-103">A *OnChange* esemény nem fordul elő, ha a mező programozás útján, az *attribútum* használatával módosul. [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) metódus.</span><span class="sxs-lookup"><span data-stu-id="4c3f1-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="4c3f1-104">Ha azt szeretné, hogy a *OnChange* eseményhez tartozó eseménykezelők futásra kerüljenek, akkor a *formcontext. Data. Entity attribútumot* kell használnia. [Fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) módszer a kódban.</span><span class="sxs-lookup"><span data-stu-id="4c3f1-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute.*[fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
