---
title: 932-es frissítés AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: ff3f74348599788edd8ce0991fe49bb6a54b55af
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506085"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="17165-102">Frissítés Azure AD csatlakozás</span><span class="sxs-lookup"><span data-stu-id="17165-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="17165-103">Azure AD csatlakozás, ami segít annak biztosítása érdekében, hogy a legújabb verzió fut, alapértelmezés szerint engedélyezve van a automatikus frissítés.</span><span class="sxs-lookup"><span data-stu-id="17165-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="17165-104">Az automatikus frissítési beállítások ellenőrzéséhez használja a **Get-ADSyncAutoUpgrade** parancsmag Azure AD PowerShell.</span><span class="sxs-lookup"><span data-stu-id="17165-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="17165-105">A parancsmag visszatér a következő értékek egyike:</span><span class="sxs-lookup"><span data-stu-id="17165-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="17165-106">**Engedélyezve**: automatikus frissítés engedélyezve van.</span><span class="sxs-lookup"><span data-stu-id="17165-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="17165-107">**Letiltva**: az automatikus frissítés le van tiltva.</span><span class="sxs-lookup"><span data-stu-id="17165-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="17165-108">**Suspended**: A rendszer már nem jogosult az automatikus frissítések.</span><span class="sxs-lookup"><span data-stu-id="17165-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="17165-109">Ez az érték nem lehet konfigurálni. azt állítja be a rendszer.</span><span class="sxs-lookup"><span data-stu-id="17165-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="17165-110">További tudnivalókért lásd: [Automatikus frissítés](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="17165-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="17165-111">Borzas AD csatlakozás legújabb verziójának letöltéséhez keresse fel [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="17165-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
