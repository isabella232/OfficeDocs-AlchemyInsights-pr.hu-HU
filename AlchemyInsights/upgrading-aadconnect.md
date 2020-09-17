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
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="95d8e-102">Az Azure AD Connect frissítése</span><span class="sxs-lookup"><span data-stu-id="95d8e-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="95d8e-103">Alapértelmezés szerint az automatikus frissítés engedélyezve van az Azure AD Connect szolgáltatásban, amely segít biztosítani, hogy a legújabb verziót használja.</span><span class="sxs-lookup"><span data-stu-id="95d8e-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="95d8e-104">Az automatikus frissítési beállítások ellenőrzéséhez használja a **Get-ADSyncAutoUpgrade** parancsmagot az Azure ad PowerShellben.</span><span class="sxs-lookup"><span data-stu-id="95d8e-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="95d8e-105">A parancsmag az alábbi értékek egyikét adja vissza:</span><span class="sxs-lookup"><span data-stu-id="95d8e-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="95d8e-106">**Engedélyezve**: az automatikus frissítés engedélyezve van.</span><span class="sxs-lookup"><span data-stu-id="95d8e-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="95d8e-107">**Letiltva**: az automatikus frissítés le van tiltva.</span><span class="sxs-lookup"><span data-stu-id="95d8e-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="95d8e-108">**Felfüggesztve**: a rendszer már nem jogosult automatikus frissítések vételére.</span><span class="sxs-lookup"><span data-stu-id="95d8e-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="95d8e-109">Ezt az értéket nem lehet konfigurálni; ezt a rendszert a rendszer adja meg.</span><span class="sxs-lookup"><span data-stu-id="95d8e-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="95d8e-110">További információt az [automatikus frissítés](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)című témakörben találhat.</span><span class="sxs-lookup"><span data-stu-id="95d8e-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="95d8e-111">Az Azure AD Connect legújabb verziójának letöltéséhez nyissa meg a lehetőséget [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .</span><span class="sxs-lookup"><span data-stu-id="95d8e-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
