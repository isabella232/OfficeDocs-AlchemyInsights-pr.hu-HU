---
title: 2491 E-mail üzenetek riasztása a "Bérlő vagy felhasználó által felülbírálása miatt kézbesített adatlopó" házirendből
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e4efd504304da757687e697ff23374aeea31851
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758930"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="e0aad-102">E-mail üzenetek riasztása a "Bérlő vagy felhasználó felülbírálása miatt kézbesített adatlopó" házirendből</span><span class="sxs-lookup"><span data-stu-id="e0aad-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="e0aad-103">A "Bérlő vagy felhasználó felülbírálása miatt kézbesített adatphish" nevű alapértelmezett riasztási szabályzat ot vezették be az Office 365 ATP P1 és P2 licenccel rendelkező bérlők számára.</span><span class="sxs-lookup"><span data-stu-id="e0aad-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="e0aad-104">Ha ezt a riasztást kapta, az alábbi lépéseket kell kivizsgálnia:</span><span class="sxs-lookup"><span data-stu-id="e0aad-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="e0aad-105">A figyelmeztető üzenetben kattintson a **Riasztás megtekintése** gombra a Biztonsági & megfelelőségi központ **Riasztások** lapjára.</span><span class="sxs-lookup"><span data-stu-id="e0aad-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="e0aad-106">Válassza ki a riasztást az **üzenetlista** megtekintéséhez vagy az Üzenetek megtekintése az **Intézőben**lehetőséghez.</span><span class="sxs-lookup"><span data-stu-id="e0aad-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="e0aad-107">Mindkét lehetőség az üzenet részleteit tartalmazza, beleértve az üzenetazonosítót is.</span><span class="sxs-lookup"><span data-stu-id="e0aad-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="e0aad-108">Vegye figyelembe, hogy a Fenyegetéskezelő hivatkozás automatikusan szűri a riasztási feltételeknek megfelelő üzeneteket.</span><span class="sxs-lookup"><span data-stu-id="e0aad-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="e0aad-109">Előfordulhat, hogy módosítania kell a dátumszűrőt a Fenyegetéskezelőben.</span><span class="sxs-lookup"><span data-stu-id="e0aad-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="e0aad-110">Az adathalász üzenetet manuálisan konfigurált felülbírálás miatt kézbesítették:</span><span class="sxs-lookup"><span data-stu-id="e0aad-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="e0aad-111">A felhasználó által beállított engedélyezett feladó vagy tartomány.</span><span class="sxs-lookup"><span data-stu-id="e0aad-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="e0aad-112">A rendszergazda által a levélszemét elleni házirendben beállított engedélyezett feladó vagy tartomány.</span><span class="sxs-lookup"><span data-stu-id="e0aad-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="e0aad-113">Engedélyezett IP-cím egy kapcsolatszűrő-házirendben.</span><span class="sxs-lookup"><span data-stu-id="e0aad-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="e0aad-114">Olyan levélforgalom-szabály (más néven átviteli szabály), amely úgy van beállítva, hogy engedélyezze az üzeneteket.</span><span class="sxs-lookup"><span data-stu-id="e0aad-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="e0aad-115">Ha úgy gondolja, hogy az üzenetet helytelenül jelölték meg adatlopóként, az Outlook [Jelentésüzenet bővítmény segítségével](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) küldjön üzenetmintákat a Microsoftnak.</span><span class="sxs-lookup"><span data-stu-id="e0aad-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
