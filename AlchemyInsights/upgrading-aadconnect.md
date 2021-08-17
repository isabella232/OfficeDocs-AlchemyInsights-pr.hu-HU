---
title: 932 Az AADConnect frissítése
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
ms.openlocfilehash: 9582f1f56e6730e35520b5d79bc245cd74bea0bf4db39b379a7cd133bafc16ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104814"
---
# <a name="upgrade-azure-ad-connect"></a>Azure AD-Csatlakozás

Alapértelmezés szerint az automatikus frissítés engedélyezve van az Azure AD Csatlakozás, amely segít biztosítani, hogy a legújabb verziót használja. Az automatikus frissítési beállítások ellenőrzéséhez használja a **Get-ADSyncAutoUpgrade** parancsmagot az Azure AD PowerShellben. A parancsmag az alábbi értékek egyikét adja vissza:

- **Engedélyezve:** Az automatikus frissítés engedélyezve van.

- **Letiltva:** Az automatikus frissítés le van tiltva.

- **Felfüggesztve:** A rendszer már nem jogosult az automatikus frissítések fogadására. Ez az érték nem konfigurálható; beállítását a rendszer adja meg.

További információ: Automatikus [frissítés.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)

Az Azure AD-szolgáltatások legújabb verziójának letöltéséhez Csatlakozás a [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) következőt: .
