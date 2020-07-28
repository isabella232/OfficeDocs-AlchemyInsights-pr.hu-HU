---
title: Több objektum identitásának ugyanaz az e-mail címe.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439193"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>Több objektum identitásának ugyanaz az e-mail címe.

**Több objektum**

A hiba egyik gyakori oka, hogy nem tudja megfelelően továbbirányítani az Outlook Web Access-kérelmeket több olyan objektum jelenlétében, amelyek azonos e-mail címmel rendelkeznek, mint az identitás. Az objektumok megkereséséhez futtassa a következő parancsokat:

· Get-címzett<email address>

· Get-felhasználó<email address>

· Get-User <email address> -SoftDeletedUser

· Kapcsolatfelvétel<email address>

· Bekéselmi láda <email address> - Nyilvános mappa

· Beget-postaláda <email address> -IncludeSoftDeletedMailbox

· Postaláda begete <email address> -InactiveMailboxOnly

A probléma megoldásához távolítson el több objektumot ugyanazzal az e-mail identitással, és győződjön meg arról, hogy egyetlen objektum van az adott e-mail identitással, és a címzett típusa UserMailbox.

**Ugyanaz a cím az üzleti és fogyasztói postaládákhoz is használható**

A másik ok az, ha ugyanazt a címet használják az üzleti és fogyasztói postaládákhoz. Ebben az esetben a felhasználónak módosítania kell az elsődleges fogyasztói aliasát, amíg a Cafe nem támogatja ezt a forgatókönyvet. Ez egy állandó hiba, amely nem megy el beavatkozás nélkül.

További információt [a Microsoft-fiók e-mail címének vagy telefonszámának módosítása című témakörben talál.](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account)