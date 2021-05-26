---
title: A végpont DLP-beállításainak konfigurálása
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657931"
---
# <a name="configure-endpoint-dlp"></a>A végpont DLP-beállításainak konfigurálása

A Microsoft Endpoint DLP lehetővé teszi a DLP-védelem és -figyelés kibővítését a Windows 10-es eszközökön lévő bizalmas információkra. Az eszközök az eszközkezelésbe való átvezetését követően adatveszteség-megelőzési házirendeket hozhat létre, hogy végrehajtsa a megfelelő műveleteket az elemeken. A Tevékenységkezelővel figyelheti a bizalmas elemek tevékenységét. További információért lásd: [Eszközök bevezetése az eszközkezelésbe](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

A végponti adatveszteség-megelőzés szolgáltatás első lépései:

- Ellenőrizze, hogy rendelkezik-e a megfelelő termékváltozatok/előfizetések licencével. További információért lásd: [Termékváltozat/előfizetés licencelés](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Ellenőrizze az eszközkezelés engedélyezéséhez, a bevezetési lap eléréséhez, illetve az eszközfigyelés be- és kikapcsolához szükséges engedélyeket. További információért lásd: [Engedélyek](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Kövesse az eszközbevezetési folyamatot az eszközök bevezetéséhez az eszközkezelésbe. További információért lásd: [Eszközök bevezetése](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Adatveszteség-megelőzési házirendek létrehozása a bizalmas elemek védelméhez. További információért lásd: [Végpont DLP-házirend forgatókönyvek](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).

A Microsoft végponti adatveszteség-megelőzés szolgáltatásról további információért lásd: [A Microsoft 365 végponti adatveszteség-megelőzés (előzetes verzió)](/microsoft-365/compliance/endpoint-dlp-learn-about).

**Fontos adatgyűjtési lépések, ha támogatás szükséges:**

1. Töltse [MDATP Client Analyzer Preview (Ügyfélanalizáló előzetes verzió) gombra.](https://aka.ms/betamdatpanalyzer)
1. Eszköz futtatása rendszergazdaként a parancsablakból:

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. Amikor a rendszer **kéri, adja** meg a nyomkövetések gyűjtéséhez szükséges percek számát: , adja meg az eset futtatásához szükséges percek számát.
1. Futtassa az esetet.

Gyűjtse össze a Zip-fájl kimenetét, és adja át a támogatási ügynöknek.
