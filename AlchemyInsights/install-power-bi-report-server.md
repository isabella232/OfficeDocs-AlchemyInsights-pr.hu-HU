---
title: A Power BI jelentéskiszolgálójának telepítése
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
- "1304"
- "2500001"
ms.openlocfilehash: 8479be2a538228b71033aca3907d3aba2f5e28fb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51832096"
---
# <a name="install-power-bi-report-server"></a><span data-ttu-id="47348-102">A Power BI jelentéskiszolgálójának telepítése</span><span class="sxs-lookup"><span data-stu-id="47348-102">Install Power BI Report Server</span></span>

1. <span data-ttu-id="47348-103">Keresse meg az PowerBIReportServer.exe helyét, és indítsa el a telepítőt.</span><span class="sxs-lookup"><span data-stu-id="47348-103">Find the location of PowerBIReportServer.exe and launch the installer.</span></span>

2. <span data-ttu-id="47348-104">Válassza **a Power BI Jelentéskiszolgáló telepítése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="47348-104">Select **Install Power BI Report Server**.</span></span>

3. <span data-ttu-id="47348-105">Válassza ki a telepíteni kívánt kiadást, majd válassza a Tovább **gombot.**</span><span class="sxs-lookup"><span data-stu-id="47348-105">Choose an edition to install and then select **Next**.</span></span>

4. <span data-ttu-id="47348-106">A legördülő menüben választhat a Kiértékelés vagy a Fejlesztői kiadás közül.</span><span class="sxs-lookup"><span data-stu-id="47348-106">You can choose either Evaluation or Developer edition from the drop down.</span></span>  <span data-ttu-id="47348-107">Ellenkező esetben a Power BI szolgáltatásból vagy a mennyiségi licencszolgáltatásból beszerzett kiszolgáló termékkulcsát adhatja meg.</span><span class="sxs-lookup"><span data-stu-id="47348-107">Otherwise, you can enter a product key for the server that you acquired from either the Power BI service or the Volume License Service Center.</span></span> <span data-ttu-id="47348-108">A termékkulcs lekért mikéntjére vonatkozó további információkért lásd a Mielőtt hozzákezd című szakaszt.</span><span class="sxs-lookup"><span data-stu-id="47348-108">For more information about how to get your product key, see the Before you begin section.</span></span> <span data-ttu-id="47348-109">Olvassa el és elfogadja a licencfeltételeket, majd válassza a Tovább **gombot.**</span><span class="sxs-lookup"><span data-stu-id="47348-109">Read and agree to the license terms and conditions, and then select **Next**.</span></span>

5. <span data-ttu-id="47348-110">A jelentéskiszolgáló-adatbázis tárolására egy adatbázismotor szükséges.</span><span class="sxs-lookup"><span data-stu-id="47348-110">You need to have a Database Engine available to store the report server database.</span></span> <span data-ttu-id="47348-111">A **Tovább gombot** választva csak a jelentéskiszolgálót telepítse.</span><span class="sxs-lookup"><span data-stu-id="47348-111">Select **Next** to install the report server only.</span></span>

6. <span data-ttu-id="47348-112">Adja meg a jelentéskiszolgáló telepítési helyét.</span><span class="sxs-lookup"><span data-stu-id="47348-112">Specify the install location for the report server.</span></span> <span data-ttu-id="47348-113">A **folytatáshoz válassza** a Telepítés lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="47348-113">Select **Install** to continue.</span></span>

7. <span data-ttu-id="47348-114">A sikeres beállítás után válassza a **Jelentéskiszolgáló konfigurálása lehetőséget** a Reporting Services Configuration Manager elindításához.</span><span class="sxs-lookup"><span data-stu-id="47348-114">After a successful setup, select **Configure Report Server** to launch the Reporting Services Configuration Manager.</span></span>

<span data-ttu-id="47348-115">A telepítéskor nincs szükség sql Server Database Engine-kiszolgálóra.</span><span class="sxs-lookup"><span data-stu-id="47348-115">You don't need a SQL Server Database Engine server available at the time of install.</span></span> <span data-ttu-id="47348-116">A Reporting Services telepítés után való beállítására szüksége lesz egy ilyen szolgáltatásra.</span><span class="sxs-lookup"><span data-stu-id="47348-116">You will need one to configure Reporting Services after install.</span></span>

<span data-ttu-id="47348-117">További információ: https://docs.microsoft.com/power-bi/report-server/install-report-server</span><span class="sxs-lookup"><span data-stu-id="47348-117">For more information: https://docs.microsoft.com/power-bi/report-server/install-report-server</span></span>
