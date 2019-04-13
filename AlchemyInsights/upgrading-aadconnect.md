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
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="32d9b-102">Frissítés Azure AD csatlakozás</span><span class="sxs-lookup"><span data-stu-id="32d9b-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="32d9b-103">Azure AD csatlakozás, ami segít annak biztosítása érdekében, hogy a legújabb verzió fut, alapértelmezés szerint engedélyezve van a automatikus frissítés.</span><span class="sxs-lookup"><span data-stu-id="32d9b-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="32d9b-104">Az automatikus frissítési beállítások ellenőrzéséhez használja a **Get-ADSyncAutoUpgrade** parancsmag Azure AD PowerShell.</span><span class="sxs-lookup"><span data-stu-id="32d9b-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="32d9b-105">A parancsmag visszatér a következő értékek egyike:</span><span class="sxs-lookup"><span data-stu-id="32d9b-105">The cmdlet will return one of following values:</span></span> 

- <span data-ttu-id="32d9b-106">**Engedélyezve**: automatikus frissítés engedélyezve van.</span><span class="sxs-lookup"><span data-stu-id="32d9b-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="32d9b-107">**Letiltva**: az automatikus frissítés le van tiltva.</span><span class="sxs-lookup"><span data-stu-id="32d9b-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="32d9b-108">**Suspended**: A rendszer már nem jogosult az automatikus frissítések.</span><span class="sxs-lookup"><span data-stu-id="32d9b-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="32d9b-109">Ez az érték nem lehet konfigurálni. azt állítja be a rendszer.</span><span class="sxs-lookup"><span data-stu-id="32d9b-109">You can't configure this value; it's set by the system.</span></span> 

<span data-ttu-id="32d9b-110">További tudnivalókért lásd: [Automatikus frissítés](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="32d9b-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="32d9b-111">Borzas AD csatlakozás legújabb verziójának letöltéséhez keresse fel [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="32d9b-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
