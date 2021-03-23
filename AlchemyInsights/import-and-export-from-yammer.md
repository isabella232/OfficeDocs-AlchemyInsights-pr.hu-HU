---
title: Importálás és exportálás a Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036124"
---
# <a name="import-and-export-from-yammer"></a><span data-ttu-id="d1c40-102">Importálás és exportálás a Yammer</span><span class="sxs-lookup"><span data-stu-id="d1c40-102">Import and export from Yammer</span></span>

<span data-ttu-id="d1c40-103">**Importálás**</span><span class="sxs-lookup"><span data-stu-id="d1c40-103">**Import**</span></span>

<span data-ttu-id="d1c40-104">A felhasználói importálási beállítások attól függően változnak, hogy Yammer a [Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)natív módjában van-e, vagy sem.</span><span class="sxs-lookup"><span data-stu-id="d1c40-104">User-import options vary depending on whether your Yammer network is in [Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), or not.</span></span>

- <span data-ttu-id="d1c40-105">**Nem natív** mód: A felhasználók importálhatók csoportokba a Hozzáadás címjegyzékből [(legfeljebb](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) 100 felhasználóval) használatával a csoportbeállítások között, illetve a hálózatba a hálózati rendszergazda tömeges frissítésével. [](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users)</span><span class="sxs-lookup"><span data-stu-id="d1c40-105">**Non-Native Mode**: Users can be imported to groups using [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limit to 100 users) within group settings, or to the network using [Bulk Update](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) within Network Admin.</span></span>
- <span data-ttu-id="d1c40-106">**Natív mód:** A csoporttagságot és a hálózati tagsági műveleteket a [Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users)Felügyeleti portálon, az [Azure AD portálon](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)vagy egy másik Azure AD-beállítással kell végrehajtani.</span><span class="sxs-lookup"><span data-stu-id="d1c40-106">**Native Mode**: Group membership and network membership operations should be performed from the [Microsoft 365 admin portal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), or using another Azure AD option.</span></span> <span data-ttu-id="d1c40-107">A natív módban található hálózatok többé nem férnek hozzá a tömeges frissítéshez és más korábbi funkciókhoz.</span><span class="sxs-lookup"><span data-stu-id="d1c40-107">Networks in Native Mode no longer have access to Bulk Update and other legacy features.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="d1c40-108">Yammer még akkor sem támogatja a tartalom importálását a hálózati rendszergazdából, ha az adatexportozási funkciót egy másik hálózaton használták.</span><span class="sxs-lookup"><span data-stu-id="d1c40-108">Yammer never supported importing content from within Network Admin even when the Data Export feature was used in another network.</span></span> <span data-ttu-id="d1c40-109">A tartalmakat újra közzétenheti partnermegoldások vagy az Yammer REST API-k.</span><span class="sxs-lookup"><span data-stu-id="d1c40-109">Content can be re-posted by partner solutions or the Yammer REST APIs.</span></span>

<span data-ttu-id="d1c40-110">**Exportálás**</span><span class="sxs-lookup"><span data-stu-id="d1c40-110">**Export**</span></span>

<span data-ttu-id="d1c40-111">[A hálózati adatok hálózati rendszergazdai](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) exportálása lehetővé teszi a tartalom exportálását Yammer hálózatokból, beleértve az üzeneteket és fájlokat is.</span><span class="sxs-lookup"><span data-stu-id="d1c40-111">[Export Network Data within Network Admin](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permits the export of content from Yammer networks, including messages and files.</span></span> <span data-ttu-id="d1c40-112">A mellékletek rendkívül nagy méretűek, és az exportálások befejeződését is jelentősen igénybe veszi.</span><span class="sxs-lookup"><span data-stu-id="d1c40-112">Attachments can be extremely large and will cause exports to take significant time to complete.</span></span> <span data-ttu-id="d1c40-113">Azt javasoljuk, hogy az aktív hálózatok exportálása az adatexportálti [API](https://developer.yammer.com/docs/data-export-api) használatával napi vagy heti adattömbökbe.</span><span class="sxs-lookup"><span data-stu-id="d1c40-113">We recommend that active networks are exported using the [Data Export API](https://developer.yammer.com/docs/data-export-api) in chunks by day or week.</span></span> <span data-ttu-id="d1c40-114">Erre a célra a Microsoft ügyfélszolgálata nem biztosít egyéni parancsfájlokat.</span><span class="sxs-lookup"><span data-stu-id="d1c40-114">Microsoft Support does not provide custom scripts for this purpose.</span></span>

<span data-ttu-id="d1c40-115">Külön [GDPR-exportálás létezik](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) a tartalmak egy adott felhasználónak való exportálására.</span><span class="sxs-lookup"><span data-stu-id="d1c40-115">A separate [GDPR export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) exists to export content for an individual user.</span></span>