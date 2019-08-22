---
title: Dynamics 365 képezi az üzleti szabályok - üzleti szabály nem Firing-űrlap
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529021"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="3b4df-102">Módosításra esemény fordul elő, ha a mező módosul programozott</span><span class="sxs-lookup"><span data-stu-id="3b4df-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="3b4df-103">A *módosításra* esemény fordul elő, ha a mező módosul a programozás útján használja a *attribútum.* [Értékbeállítás](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) módszer.</span><span class="sxs-lookup"><span data-stu-id="3b4df-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="3b4df-104">Ha azt szeretné futtatni kell használni az érték beállítása után a *módosításra* esemény eseménykezelők a *attribútum formContext.data.entity.* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) módszer a kódban.</span><span class="sxs-lookup"><span data-stu-id="3b4df-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute.*[fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
