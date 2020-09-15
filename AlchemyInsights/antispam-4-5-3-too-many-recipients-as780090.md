---
title: a 1049 AntiSpam 4.5.3 túl sok címzett (AS780090)
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
- "1049"
- "3100024"
ms.assetid: fa3d4be9-c90a-4926-9754-4b708b038bf6
ms.openlocfilehash: deb57e6e872ce5769a339c7d130a63a8e90ab4c8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717795"
---
# <a name="453-too-many-recipients-as780090"></a><span data-ttu-id="112bd-102">túl sok címzett 4.5.3 (AS780090)</span><span class="sxs-lookup"><span data-stu-id="112bd-102">4.5.3 Too many recipients (AS780090)</span></span>

<span data-ttu-id="112bd-103">Ez a hiba akkor fordul elő, ha a forrás IP-címről érkező e-mail-forgalom mennyisége meghaladja a forrás IP-címének jó hírneve (vagy a jó hírneve hiánya) alapján megadott korlátot.</span><span class="sxs-lookup"><span data-stu-id="112bd-103">This error occurs when the volume of email traffic from the source IP address exceeds the limit based on the reputation (or lack of reputation) of source IP address.</span></span>

<span data-ttu-id="112bd-104">A forrás IP-címről érkező e-mailek blokkolása egy órán belül lejár.</span><span class="sxs-lookup"><span data-stu-id="112bd-104">Blocking email from the source IP address will expire within an hour.</span></span> <span data-ttu-id="112bd-105">Ha a forrás IP-címe egy olyan helyszíni levelezési kiszolgáló, amely az Ön tulajdonában van, ellenőrizze az e-mail-forgalom összekötő konfigurációját.</span><span class="sxs-lookup"><span data-stu-id="112bd-105">If the source IP address is an on-premises email server that belongs to you, verify the configuration of the mail flow connector.</span></span> <span data-ttu-id="112bd-106">Ha a viselkedés több mint egy órára továbbra is fennáll, akkor az ügyfélszolgálattól kérhet kivételt a forrás IP-címéhez.</span><span class="sxs-lookup"><span data-stu-id="112bd-106">If the behavior continues for more than an hour, contact support to request an exception for the source IP address.</span></span>
