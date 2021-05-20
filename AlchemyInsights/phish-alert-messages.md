---
title: '2491: E-mailek értesítése a "Kézbesítésről bérlő vagy felhasználó felülbírálása miatt" házirendről'
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2b373423cf3e63b76a62465dd62076c023580e94
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544580"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="db1b2-102">E-mail üzenetek riasztása a "Kézbesítés a bérlő vagy a felhasználó felülbírálása miatt" házirendből</span><span class="sxs-lookup"><span data-stu-id="db1b2-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="db1b2-103">A Microsoft Defender Office 365 P1 és P2 licenccel rendelkező bérlői fiókokban egy alapértelmezett "Kézbesítés bérlői fiók vagy felhasználói felülbírálás miatt" nevű riasztási házirendet hoztunk létre.</span><span class="sxs-lookup"><span data-stu-id="db1b2-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Microsoft Defender for Office 365 P1 and P2 licenses.</span></span> <span data-ttu-id="db1b2-104">Ha megkapta ezt a riasztást, az alábbi lépéseket kell vizsgálnia:</span><span class="sxs-lookup"><span data-stu-id="db1b2-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="db1b2-105">A riasztási üzenetben kattintson a  Riasztás megtekintése elemre a Biztonsági megfelelőségi központ Riasztások & lapjára való ugráshoz. </span><span class="sxs-lookup"><span data-stu-id="db1b2-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="db1b2-106">A figyelmeztetést választva megtekintheti az Üzenetlista megtekintése **vagy** az **Üzenetek megtekintése Intézőben lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="db1b2-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="db1b2-107">Mindkét lehetőséggel az üzenet részleteire megjelenik, amely tartalmazza az üzenetazonosítót.</span><span class="sxs-lookup"><span data-stu-id="db1b2-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="db1b2-108">Vegye figyelembe, hogy a Veszélyforrás-intéző hivatkozás automatikusan szűri a riasztási feltételeknek megfelelő üzeneteket.</span><span class="sxs-lookup"><span data-stu-id="db1b2-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="db1b2-109">Előfordulhat, hogy módosítania kell a dátumszűrőt a Veszélyforrás-intézőben.</span><span class="sxs-lookup"><span data-stu-id="db1b2-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="db1b2-110">Az adathalász üzenet kézbesítése egy kézzel konfigurált felülbírálás miatt történt:</span><span class="sxs-lookup"><span data-stu-id="db1b2-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="db1b2-111">A felhasználó által beállított engedélyezett feladó vagy tartomány.</span><span class="sxs-lookup"><span data-stu-id="db1b2-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="db1b2-112">A rendszergazda által egy levélszemét elleni házirendben beállított engedélyezett feladó vagy tartomány.</span><span class="sxs-lookup"><span data-stu-id="db1b2-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="db1b2-113">Egy kapcsolatszűrő házirendben engedélyezett IP-cím.</span><span class="sxs-lookup"><span data-stu-id="db1b2-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="db1b2-114">Egy olyan e-mail-forgalom szabály (más néven átviteli szabály), amely az üzenetek fogadására van beállítva.</span><span class="sxs-lookup"><span data-stu-id="db1b2-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="db1b2-115">Ha úgy véli, hogy az üzenetet helytelenül jelölte [](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) meg phish Outlook, az "Üzenet bejelentése" bővítmény használatával küldje el az üzenetmintákat a Microsoftnak.</span><span class="sxs-lookup"><span data-stu-id="db1b2-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
