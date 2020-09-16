---
title: az 2491 riasztási e-mail-üzeneteket a bérlői fiók vagy a felhasználó felülírása házirend szerint
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
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728613"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="c8fb5-102">E-mail-üzenetek küldése a bérlői fiók vagy a felhasználó felülírása házirend által kiszállított adathalászó számára</span><span class="sxs-lookup"><span data-stu-id="c8fb5-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="c8fb5-103">A bérlői fiók vagy a felhasználó felülírása "az adathalászók számára kiszállítva" nevű alapértelmezett riasztási házirendet a bérlők az ATP P1 és 365 a P2 licenccel rendelkező bérlői fiókba építették.</span><span class="sxs-lookup"><span data-stu-id="c8fb5-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="c8fb5-104">Ha ezt az értesítést kapta, az alábbi lépéseket követve vizsgálja meg:</span><span class="sxs-lookup"><span data-stu-id="c8fb5-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="c8fb5-105">A riasztási üzenetben az értesítés **megtekintése** gombra kattintva nyissa meg az **értesítések** lapot a biztonsági & megfelelőségi központban.</span><span class="sxs-lookup"><span data-stu-id="c8fb5-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="c8fb5-106">A riasztás elemre koppintva megtekintheti az **üzenetlistában megtekinthető** és az **üzenetek megtekintése az Intézőben**című témakört.</span><span class="sxs-lookup"><span data-stu-id="c8fb5-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="c8fb5-107">Mindkét beállítással megadhatja az üzenet részleteit, beleértve az üzenet AZONOSÍTÓját is.</span><span class="sxs-lookup"><span data-stu-id="c8fb5-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="c8fb5-108">Fontos tudni, hogy a fenyegetések Explorer hivatkozása automatikusan szűri az értesítési feltételnek megfelelő üzeneteket.</span><span class="sxs-lookup"><span data-stu-id="c8fb5-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="c8fb5-109">Előfordulhat, hogy módosítania kell a szűrőt a fenyegetések Explorerben.</span><span class="sxs-lookup"><span data-stu-id="c8fb5-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="c8fb5-110">Az adathalászati üzenet a manuálisan konfigurált felülbírálás miatt lett kézbesítve:</span><span class="sxs-lookup"><span data-stu-id="c8fb5-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="c8fb5-111">A felhasználó által beállított engedélyezett feladó vagy tartomány.</span><span class="sxs-lookup"><span data-stu-id="c8fb5-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="c8fb5-112">Egy levélszemét elleni házirendben a rendszergazda által beállított engedélyezett feladó vagy tartomány.</span><span class="sxs-lookup"><span data-stu-id="c8fb5-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="c8fb5-113">Egy engedélyezett IP-cím a kapcsolati szűrő házirendjében.</span><span class="sxs-lookup"><span data-stu-id="c8fb5-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="c8fb5-114">E-mail-forgalom szabálya (más néven átviteli szabály), amely az üzenetek engedélyezésére van konfigurálva.</span><span class="sxs-lookup"><span data-stu-id="c8fb5-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="c8fb5-115">Ha úgy véli, hogy az üzenet tévesen volt megjelölve adathalászként, az Outlook [-jelentés üzenet bővítményével](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) elküldheti az üzenet mintáit a Microsoftnak.</span><span class="sxs-lookup"><span data-stu-id="c8fb5-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
