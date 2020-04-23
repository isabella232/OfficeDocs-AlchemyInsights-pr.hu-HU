---
title: 932 Az AADConnect frissítése
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766495"
---
# <a name="upgrade-azure-ad-connect"></a>Az Azure AD Connect frissítése

Alapértelmezés szerint az automatikus frissítés engedélyezve van az Azure AD Connect, amely segít biztosítani, hogy a legújabb verziót fut. Az automatikus frissítési beállítások ellenőrzéséhez használja a **Get-ADSyncAutoUpgrade** parancsmag az Azure AD PowerShellben. A parancsmag a következő értékek egyikét adja vissza:

- **Engedélyezve**: Az automatikus frissítés engedélyezve van.

- **Letiltva**: Az automatikus frissítés le van tiltva.

- **Felfüggesztve**: A rendszer már nem jogosult automatikus frissítésekre. Ez az érték nem konfigurálható; A rendszer állítja be.

További információt az [Automatikus frissítés](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)című témakörben talál.

Az Azure AD Connect legújabb verziójának [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)letöltéséhez nyissa meg a.y
