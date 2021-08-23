---
title: Az alkalmazás nem jelenik meg az App irányításában
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12734"
ms.openlocfilehash: a8d176fdee073e41b61de6f53c728601da955aaa
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/16/2021
ms.locfileid: "58454697"
---
# <a name="my-app-isnt-showing-up-in-app-governance"></a>Az alkalmazás nem jelenik meg az App irányításában

Ha az alkalmazás nem jelenik meg az App irányításában, ellenőrizze az alábbiakat:

1. Keresse fel [az Azure AD webhelyet,](https://aad.portal.azure.com/) és keresse meg az alkalmazás alkalmazásazonosítóját, ha rákeres az app nevére az Áttekintés lap felső sávján.

1. Az access Graph Explorerben, és keresse meg az appazonosítót a egyszerű szolgáltatásnévben a lekérdezés használatával, és cserélje le a megfelelő appazonosítóra: <appId> < https://graph.microsoft.com/v1.0/servicePrincipals? $search= "appId: <appId> ">

1. Ha nem ad vissza találatot, keresse meg az appazonosítót az alkalmazáson belül a következő lekérdezés használatával, és cserélje le a megfelelő appazonosítót: <appId> < https://graph.microsoft.com/v1.0/applications? $search= "appAzonosító: <appId> ">

Ha problémákat tapasztal a lekérdezéssel kapcsolatban, lásd: [Támogatás](https://docs.microsoft.com/microsoft-365/business-video/get-help-support) 

Az appok irányításában való alkalmazásokkal kapcsolatos további információkért és információkért lásd: Információk a [láthatóságról és az összefüggésekről.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-overview)

Az alkalmazások megtekintéséről további információt Az [alkalmazások megtekintése.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-view-apps)
