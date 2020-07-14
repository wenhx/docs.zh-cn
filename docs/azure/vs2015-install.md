---
title: 用于 Visual Studio 2015 的 Azure 工具
description: 获取工具以开始使用 Visual Studio 2015 中的 Azure .NET 库。
ms.date: 06/19/2020
ms.custom: azure-sdk-dotnet
ms.openlocfilehash: 72229ce0c0276912ddc5658e34f4572a7948a4e6
ms.sourcegitcommit: cb27c01a8b0b4630148374638aff4e2221f90b22
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2020
ms.locfileid: "86174818"
---
# <a name="azure-tools-for-visual-studio-2015"></a><span data-ttu-id="19bbc-103">用于 Visual Studio 2015 的 Azure 工具</span><span class="sxs-lookup"><span data-stu-id="19bbc-103">Azure tools for Visual Studio 2015</span></span>

<span data-ttu-id="19bbc-104">安装**用于 Visual Studio 2015 的 Azure SDK** 以及**用于 Visual Studio 2015 的 Service Fabric SDK 和工具**的最快、最简单方法是使用 [Web 平台安装程序](https://www.microsoft.com/web/downloads/platform.aspx)。</span><span class="sxs-lookup"><span data-stu-id="19bbc-104">The quickest and easiest way to install the **Azure SDK for Visual Studio 2015** and **Service Fabric SDK and Tools for Visual Studio 2015** is using the [Web Platform Installer](https://www.microsoft.com/web/downloads/platform.aspx).</span></span> <span data-ttu-id="19bbc-105">Microsoft Web 平台安装程序是一个免费工具，可简化 Microsoft Web 平台的某些组件（包括用于 Visual Studio 2015 的 Azure 工具）的下载、安装和更新。</span><span class="sxs-lookup"><span data-stu-id="19bbc-105">The Microsoft Web Platform Installer is a free tool that streamlines downloading, installing, and updating some of the components of the Microsoft Web Platform, including Azure tools for Visual Studio 2015.</span></span> <span data-ttu-id="19bbc-106">也可以从 [Azure 下载页](https://azure.microsoft.com/downloads/)以独立组件的形式下载并安装这些 SDK。</span><span class="sxs-lookup"><span data-stu-id="19bbc-106">These SDKs can also be downloaded and installed as individual components from the [Azure Downloads page](https://azure.microsoft.com/downloads/).</span></span>

## <a name="using-the-web-platform-installer"></a><span data-ttu-id="19bbc-107">使用 Web 平台安装程序</span><span class="sxs-lookup"><span data-stu-id="19bbc-107">Using the Web Platform Installer</span></span>

1. <span data-ttu-id="19bbc-108">下载并运行此 [Web 平台安装程序引导程序](https://www.microsoft.com/web/handlers/webpi.ashx?command=getinstallerredirect&appid=VWDOrVs2015AzurePack;MicrosoftAzure-ServiceFabric-VS2015)。</span><span class="sxs-lookup"><span data-stu-id="19bbc-108">Download and run this [Web Platform Installer bootstrapper](https://www.microsoft.com/web/handlers/webpi.ashx?command=getinstallerredirect&appid=VWDOrVs2015AzurePack;MicrosoftAzure-ServiceFabric-VS2015).</span></span>

2. <span data-ttu-id="19bbc-109">该引导程序会安装 Web 平台安装程序（如果需要），并自动将最新版本的**用于 Visual Studio 2015 的 Azure SDK** 以及**用于 Visual Studio 2015 的 Service Fabric SDK 和工具**项放入“要安装的项”列表中。 </span><span class="sxs-lookup"><span data-stu-id="19bbc-109">The bootstrapper will install Web Platform Installer (if needed) and automatically put the latest versions of the  **Azure SDK for Visual Studio 2015** and **Service Fabric SDK and Tools for Visual Studio 2015** items in your *Items to be installed* list.</span></span> <span data-ttu-id="19bbc-110">单击“安装”  。</span><span class="sxs-lookup"><span data-stu-id="19bbc-110">Click **Install**.</span></span>

    ![Web 平台安装程序](media/vs2015-install/webpi.png)

3. <span data-ttu-id="19bbc-112">在下一屏幕中，单击“我接受”。 </span><span class="sxs-lookup"><span data-stu-id="19bbc-112">On the next screen, click **I Accept**.</span></span> <span data-ttu-id="19bbc-113">Web PI 会开始下载并安装所选的组件。</span><span class="sxs-lookup"><span data-stu-id="19bbc-113">Web PI will begin downloading and installing the components you selected.</span></span>

4. <span data-ttu-id="19bbc-114">安装完成后，会显示确认屏幕。</span><span class="sxs-lookup"><span data-stu-id="19bbc-114">After the installation is finished, it will display a confirmation screen.</span></span> <span data-ttu-id="19bbc-115">单击 **“完成”** 。</span><span class="sxs-lookup"><span data-stu-id="19bbc-115">Click **Finish**.</span></span> <span data-ttu-id="19bbc-116">现在可以关闭 Web 平台安装程序。</span><span class="sxs-lookup"><span data-stu-id="19bbc-116">You can now close Web Platform Installer.</span></span>

## <a name="verifying-the-installation"></a><span data-ttu-id="19bbc-117">验证安装</span><span class="sxs-lookup"><span data-stu-id="19bbc-117">Verifying the installation</span></span>

1. <span data-ttu-id="19bbc-118">在 Visual Studio 2015 中，依次单击“工具”菜单、“扩展和更新...”。  </span><span class="sxs-lookup"><span data-stu-id="19bbc-118">In Visual Studio 2015, click the **Tools** menu, and then click **Extensions and Updates...**.</span></span>

2. <span data-ttu-id="19bbc-119">显示的列表包含多个 Azure 工具，例如“Microsoft Azure 应用服务工具”、“Microsoft Azure 存储连接服务”和“Service Fabric 工具”。   </span><span class="sxs-lookup"><span data-stu-id="19bbc-119">The displayed list will contain several Azure tools, such as **Microsoft Azure App Service Tools**, **Microsoft Azure Storage Connected Service**, and **Service Fabric Tools**.</span></span>

    ![扩展和更新](media/vs2015-install/ext-tools.png)