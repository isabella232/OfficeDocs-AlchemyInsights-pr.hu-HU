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
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/25/2019
ms.locfileid: "36529021"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>A OnChange esemény nem következik be, ha a mező programozás útján módosul

A *OnChange* esemény nem fordul elő, ha a mező programozás útján, az *attribútum* használatával módosul. [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) metódus. Ha azt szeretné, hogy a *OnChange* eseményhez tartozó eseménykezelők futásra kerüljenek, akkor a *formcontext. Data. Entity attribútumot* kell használnia. [Fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) módszer a kódban.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
