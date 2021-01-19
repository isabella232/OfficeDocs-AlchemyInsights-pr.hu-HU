---
title: Felhasználó beleegyezésével kapcsolatos hibák elhárítása
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7785"
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901190"
---
# <a name="troubleshoot-user-consent"></a>Felhasználó beleegyezésével kapcsolatos hibák elhárítása

1. Beállíthatja, hogy a végfelhasználók hogyan járulnak hozzá az alkalmazásokhoz az Azure Portalon vagy a PowerShellen keresztül. További [információért tekintse](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) meg a felhasználói hozzájárulási beállításokat.
1. A rendszergazdák a [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) használatával is engedélyt adhatnak a delegált engedélyekhez egyetlen felhasználó nevében. További információt a [Hozzáférés lekérte egy](https://docs.microsoft.com/graph/auth-v2-user)felhasználó nevében.
1. [Felhasználói jóváhagyási hibák:](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)Ez a cikk az alkalmazásokhoz való beleegyezés során előforduló hibákat ismerteti. Ha hibaüzenetet nem tartalmazó váratlan jóváhagyási kéréseket hárít el, tekintse át az Azure AD hitelesítési [forgatókönyveit.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)