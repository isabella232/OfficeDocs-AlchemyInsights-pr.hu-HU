---
title: 932-es frissítés AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 8ffa8f64019077034bc4fad61d1d843849c42898
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/13/2019
ms.locfileid: "31858962"
---
# <a name="upgrade-azure-ad-connect"></a>Frissítés Azure AD csatlakozás

Azure AD csatlakozás, ami segít annak biztosítása érdekében, hogy a legújabb verzió fut, alapértelmezés szerint engedélyezve van a automatikus frissítés. Az automatikus frissítési beállítások ellenőrzéséhez használja a **Get-ADSyncAutoUpgrade** parancsmag Azure AD PowerShell. A parancsmag visszatér a következő értékek egyike: 

- **Engedélyezve**: automatikus frissítés engedélyezve van.

- **Letiltva**: az automatikus frissítés le van tiltva.

- **Suspended**: A rendszer már nem jogosult az automatikus frissítések. Ez az érték nem lehet konfigurálni. azt állítja be a rendszer. 

További tudnivalókért lásd: [Automatikus frissítés](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Borzas AD csatlakozás legújabb verziójának letöltéséhez keresse fel [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).
