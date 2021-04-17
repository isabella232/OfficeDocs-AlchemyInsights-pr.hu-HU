---
title: Csatlakozás az MSCommerce modulhoz
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3528"
ms.openlocfilehash: e77c6a329ac99a4cea4f143dcb3c661b6a518e35
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817030"
---
# <a name="connect-to-the-mscommerce-module"></a><span data-ttu-id="15936-102">Csatlakozás az MSCommerce modulhoz</span><span class="sxs-lookup"><span data-stu-id="15936-102">Connect to the MSCommerce module</span></span>

<span data-ttu-id="15936-103">Az AllowSelfServicePurchase házirend megtekintéséhez vagy beállításéhez csatlakoztatnia kell az MSCommerce modult.</span><span class="sxs-lookup"><span data-stu-id="15936-103">You must be connected to the MSCommerce module before you can view or set the AllowSelfServicePurchase policy.</span></span>  

<span data-ttu-id="15936-104">Az MSCommerce modulhoz való csatlakozáshoz a PowerShell parancssorában (PS C: , írja be \) a következő parancsot:</span><span class="sxs-lookup"><span data-stu-id="15936-104">To connect to the MSCommerce module, at the PowerShell prompt (PS C:\), enter the following command:</span></span>

`Connect-MSCommerce`

<span data-ttu-id="15936-105">Ezzel megnyitja a bejelentkezési párbeszédpanelt.</span><span class="sxs-lookup"><span data-stu-id="15936-105">This will open a sign-in dialog.</span></span> <span data-ttu-id="15936-106">A bejelentkezéshez adja meg a felhasználónevét és a jelszavát.</span><span class="sxs-lookup"><span data-stu-id="15936-106">Enter your username and password to sign-in.</span></span>

<span data-ttu-id="15936-107">**MEGJEGYZÉS:** &nbsp; &nbsp; A bejelentkezéshez használt fióknak vállalati vagy számlázási rendszergazdának kell lennie.</span><span class="sxs-lookup"><span data-stu-id="15936-107">**NOTE:**&nbsp;&nbsp;The account used to sign in must be a Company or Billing Administrator.</span></span>
