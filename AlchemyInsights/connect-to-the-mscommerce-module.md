---
title: Csatlakozás a MSCommerce modulhoz
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3528"
ms.openlocfilehash: 41dd044d99d14f25ea15699bfb74f7c37e3928c1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713240"
---
# <a name="connect-to-the-mscommerce-module"></a><span data-ttu-id="e88b0-102">Csatlakozás a MSCommerce modulhoz</span><span class="sxs-lookup"><span data-stu-id="e88b0-102">Connect to the MSCommerce module</span></span>

<span data-ttu-id="e88b0-103">A AllowSelfServicePurchase házirend megtekintése vagy beállítása előtt csatlakoznia kell a MSCommerce modulhoz.</span><span class="sxs-lookup"><span data-stu-id="e88b0-103">You must be connected to the MSCommerce module before you can view or set the AllowSelfServicePurchase policy.</span></span>  

<span data-ttu-id="e88b0-104">A MSCommerce modulhoz való csatlakozáshoz a PowerShell parancssorába (PS C:) \) írja be a következő parancsot:</span><span class="sxs-lookup"><span data-stu-id="e88b0-104">To connect to the MSCommerce module, at the PowerShell prompt (PS C:\), enter the following command:</span></span>

`Connect-MSCommerce`

<span data-ttu-id="e88b0-105">Ekkor megnyílik a bejelentkezési párbeszédpanel.</span><span class="sxs-lookup"><span data-stu-id="e88b0-105">This will open a sign-in dialog.</span></span> <span data-ttu-id="e88b0-106">Adja meg a felhasználónevét és a jelszavát a bejelentkezéshez.</span><span class="sxs-lookup"><span data-stu-id="e88b0-106">Enter your username and password to sign-in.</span></span>

<span data-ttu-id="e88b0-107">**Megjegyzés:** &nbsp; &nbsp; A bejelentkezéshez használt fióknak vállalati vagy számlázási rendszergazdának kell lennie.</span><span class="sxs-lookup"><span data-stu-id="e88b0-107">**NOTE:**&nbsp;&nbsp;The account used to sign in must be a Company or Billing Administrator.</span></span>
