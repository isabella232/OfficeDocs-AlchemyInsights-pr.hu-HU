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
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402427"
---
# <a name="configure-endpoint-dlp"></a>A végpont DLP-beállításainak konfigurálása

A Microsoft Endpoint DLP lehetővé teszi a DLP-védelem és -figyelés kibővítését a Windows 10-es eszközökön lévő bizalmas információkra. Az eszközök az eszközkezelésbe való átvezetését követően adatveszteség-megelőzési házirendeket hozhat létre, hogy végrehajtsa a megfelelő műveleteket az elemeken. A Tevékenységkezelővel figyelheti a bizalmas elemek tevékenységét. További információért lásd: [Eszközök bevezetése az eszközkezelésbe](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

A végponti adatveszteség-megelőzés szolgáltatás első lépései:

- Ellenőrizze, hogy rendelkezik-e a megfelelő termékváltozatok/előfizetések licencével. További információért lásd: [Termékváltozat/előfizetés licencelés](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Ellenőrizze az eszközkezelés engedélyezéséhez, a bevezetési lap eléréséhez, illetve az eszközfigyelés be- és kikapcsolához szükséges engedélyeket. További információért lásd: [Engedélyek](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Kövesse az eszközbevezetési folyamatot az eszközök bevezetéséhez az eszközkezelésbe. Ha az Eszközbevezetés (előzetes verzió) lehetőség hiányzik az M365 megfelelőségi **Beállítások** közül, erősítse meg, hogy rendelkezik a fent felsorolt megfelelő licencekkel és engedélyekkel. További információért lásd: [Eszközök bevezetése](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Adatveszteség-megelőzési házirendek létrehozása a bizalmas elemek védelméhez. További információért lásd: [Végpont DLP-házirend forgatókönyvek](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).

A Microsoft végponti adatveszteség-megelőzés szolgáltatásról további információért lásd: [A Microsoft 365 végponti adatveszteség-megelőzés (előzetes verzió)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Fontos adatgyűjtési lépések, ha támogatás szükséges:**

1. MDATP ügyfél elemző előnézet letöltése innen: [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")
2. Eszköz futtatása rendszergazdaként a parancsablakból:
3. MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t
4. Amikor az "Adja meg a nyomkövetési percek számát:" kérés jelenik meg, adja meg, hogy hány perc szükséges az eset futtatásához.
5. Eset futtatása

Gyűjtse össze a támogatási szakembernek adandó zip fájl kimenetét.
