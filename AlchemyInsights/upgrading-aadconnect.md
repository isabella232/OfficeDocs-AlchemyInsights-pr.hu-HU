---
title: 932-AADConnect frissítése
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806041"
---
# <a name="upgrade-azure-ad-connect"></a>Az Azure AD Connect frissítése

Alapértelmezés szerint az automatikus frissítés engedélyezve van az Azure AD Connect szolgáltatásban, amely segít biztosítani, hogy a legújabb verziót használja. Az automatikus frissítési beállítások ellenőrzéséhez használja a **Get-ADSyncAutoUpgrade** parancsmagot az Azure ad PowerShellben. A parancsmag az alábbi értékek egyikét adja vissza:

- **Engedélyezve**: az automatikus frissítés engedélyezve van.

- **Letiltva**: az automatikus frissítés le van tiltva.

- **Felfüggesztve**: a rendszer már nem jogosult automatikus frissítések vételére. Ezt az értéket nem lehet konfigurálni; ezt a rendszert a rendszer adja meg.

További információt az [automatikus frissítés](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)című témakörben találhat.

Az Azure AD Connect legújabb verziójának letöltéséhez nyissa meg a lehetőséget [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
