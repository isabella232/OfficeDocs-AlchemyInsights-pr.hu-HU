---
title: 1374 két postaláda – howto megoldása
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
- "1374"
- "2692"
- "3500014"
ms.assetid: 8bf1a8f2-58ef-4697-b9c0-be340de96bfe
ms.openlocfilehash: 048c527b26d138535550b5bae399d0ce9fbce0a6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720900"
---
# <a name="a-user-has-two-mailboxes"></a>Egy felhasználó két postaládával rendelkezik

Előfordulhat, hogy az Azure Active Directory Connect (AAD Connect) vagy az rSync szolgáltatást használó hibrid környezetekben a felhasználók két postaládában: egy helyszíni, a felhőben pedig egy. Bármely helyről duplikált postaládát hozhat létre.

A probléma megoldásához tekintse át, hogy [miként állíthatja helyre a postaládát, ha az Exchange Online-ban és a helyszíni webhelyen is megtalálható](https://docs.microsoft.com/exchange/troubleshoot/move-mailboxes/mailbox-exists-exo-onpremises). Ha többet szeretne megtudni arról, hogy miként kerülheti el ezt a folyamatot a jövőben, akkor olvassa el a következő témakört: [a felhasználó postaládája mind helyszíni, mind az Exchange Online-ban megtalálható. Súgó!](https://techcommunity.microsoft.com/t5/Exchange-Team-Blog/My-user-has-a-mailbox-both-on-premises-and-in-Exchange-Online/ba-p/846809).
