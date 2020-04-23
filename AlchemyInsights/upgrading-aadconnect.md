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
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="f72df-102">Az Azure AD Connect frissítése</span><span class="sxs-lookup"><span data-stu-id="f72df-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="f72df-103">Alapértelmezés szerint az automatikus frissítés engedélyezve van az Azure AD Connect, amely segít biztosítani, hogy a legújabb verziót fut.</span><span class="sxs-lookup"><span data-stu-id="f72df-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="f72df-104">Az automatikus frissítési beállítások ellenőrzéséhez használja a **Get-ADSyncAutoUpgrade** parancsmag az Azure AD PowerShellben.</span><span class="sxs-lookup"><span data-stu-id="f72df-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="f72df-105">A parancsmag a következő értékek egyikét adja vissza:</span><span class="sxs-lookup"><span data-stu-id="f72df-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="f72df-106">**Engedélyezve**: Az automatikus frissítés engedélyezve van.</span><span class="sxs-lookup"><span data-stu-id="f72df-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="f72df-107">**Letiltva**: Az automatikus frissítés le van tiltva.</span><span class="sxs-lookup"><span data-stu-id="f72df-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="f72df-108">**Felfüggesztve**: A rendszer már nem jogosult automatikus frissítésekre.</span><span class="sxs-lookup"><span data-stu-id="f72df-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="f72df-109">Ez az érték nem konfigurálható; A rendszer állítja be.</span><span class="sxs-lookup"><span data-stu-id="f72df-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="f72df-110">További információt az [Automatikus frissítés](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="f72df-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="f72df-111">Az Azure AD Connect legújabb verziójának [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)letöltéséhez nyissa meg a.y</span><span class="sxs-lookup"><span data-stu-id="f72df-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
