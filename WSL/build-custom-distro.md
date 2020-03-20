---
title: Erstellen einer benutzerdefinierten Linux-Distribution für WSL
description: Erfahren Sie, wie Sie eine benutzerdefinierte Linux-Distribution für das Windows-Subsystem für Linux erstellen.
keywords: Bashonwindows, bash, WSL, Windows, Windows Subsystem, Distribution, Custom
ms.date: 03/27/2018
ms.topic: article
ms.assetid: a5095219-0c82-4ce5-9a6d-5c2fc00835a3
ms.custom: seodec18
ms.openlocfilehash: 181badd4ee2f69e904099c12b54dfbdf3a37e294
ms.sourcegitcommit: 0b5a9f8982dfff07fc8df32d74d97293654f8e12
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/25/2019
ms.locfileid: "71269703"
---
# <a name="creating-a-custom-linux-distro-for-wsl"></a><span data-ttu-id="76c33-104">Erstellen einer benutzerdefinierten Linux-Distribution für WSL</span><span class="sxs-lookup"><span data-stu-id="76c33-104">Creating a Custom Linux Distro for WSL</span></span>

<span data-ttu-id="76c33-105">Verwenden Sie das Open Source-WSL-Beispiel, um WSL-Distributionen für das Microsoft Store zu erstellen und/oder um benutzerdefinierte Linux-Distribution-Pakete für das Sideloading zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="76c33-105">Use our open source WSL sample to build WSL distro packages for the Microsoft Store and/or to create custom Linux distro packages for sideloading.</span></span> <span data-ttu-id="76c33-106">Das Repository für [Distribution](https://github.com/Microsoft/WSL-DistroLauncher) -Start Programm finden Sie auf GitHub.</span><span class="sxs-lookup"><span data-stu-id="76c33-106">You can find the [distro launcher repo](https://github.com/Microsoft/WSL-DistroLauncher) on GitHub.</span></span>

<span data-ttu-id="76c33-107">Dieses Projekt aktiviert Folgendes:</span><span class="sxs-lookup"><span data-stu-id="76c33-107">This project enables:</span></span>
* <span data-ttu-id="76c33-108">Linux-Verteilungs-Maintainer zum Verpacken und Übermitteln einer Linux-Distribution als AppX, die auf WSL ausgeführt wird</span><span class="sxs-lookup"><span data-stu-id="76c33-108">Linux distribution maintainers to package and submit a Linux distribution as an appx that runs on WSL</span></span>
* <span data-ttu-id="76c33-109">Entwickler zum Erstellen von benutzerdefinierten Linux-Distributionen, die auf ihren Entwicklungs Computer quer geladen werden können</span><span class="sxs-lookup"><span data-stu-id="76c33-109">Developers to create custom Linux distributions that can be sideloaded onto their dev machine</span></span>

## <a name="background"></a><span data-ttu-id="76c33-110">Hintergrund</span><span class="sxs-lookup"><span data-stu-id="76c33-110">Background</span></span>
<span data-ttu-id="76c33-111">Wir verteilen Linux-Distributionen für WSL als UWP-Anwendungen über die Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="76c33-111">We distribute Linux distros for WSL as UWP applications through the Microsoft Store.</span></span> <span data-ttu-id="76c33-112">Sie können diese Anwendungen installieren, die dann auf WSL ausgeführt werden: das Subsystem, das sich im Windows-Kernel befindet.</span><span class="sxs-lookup"><span data-stu-id="76c33-112">You can install those applications that will then run on WSL - the subsystem that sits in the Windows kernel.</span></span> <span data-ttu-id="76c33-113">Dieser Übermittlungs Mechanismus hat viele Vorteile, wie in einem [früheren Blogbeitrag](https://blogs.msdn.microsoft.com/commandline/2017/07/10/ubuntu-now-available-from-the-windows-store/)erläutert.</span><span class="sxs-lookup"><span data-stu-id="76c33-113">This delivery mechanism has many benefits as discussed in an [earlier blog post](https://blogs.msdn.microsoft.com/commandline/2017/07/10/ubuntu-now-available-from-the-windows-store/).</span></span>

## <a name="sideloading-a-custom-linux-distro-package"></a><span data-ttu-id="76c33-114">Querladen eines benutzerdefinierten Linux-Distribution-Pakets</span><span class="sxs-lookup"><span data-stu-id="76c33-114">Sideloading a Custom Linux Distro Package</span></span>
<span data-ttu-id="76c33-115">Sie können ein benutzerdefiniertes Linux-Distributionspaket als Anwendung zum querladen auf Ihren persönlichen Computer erstellen.</span><span class="sxs-lookup"><span data-stu-id="76c33-115">You can create a custom Linux distro package as an application to sideload on your personal machine.</span></span> <span data-ttu-id="76c33-116">Beachten Sie, dass das benutzerdefinierte Paket nicht über das Microsoft Store verteilt wird, es sei denn, Sie übermitteln als Verteilungs Maintainer.</span><span class="sxs-lookup"><span data-stu-id="76c33-116">Please note that your custom package would not be distributed through the Microsoft Store unless you submit as a distribution maintainer.</span></span>
<span data-ttu-id="76c33-117">Wenn Sie Ihren Computer zum querladen von apps einrichten möchten, müssen Sie diesen in den Systemeinstellungen unter "für Entwickler" aktivieren.</span><span class="sxs-lookup"><span data-stu-id="76c33-117">To set up your machine to sideload apps, you will need to enable this in the system settings under “For Developers”.</span></span>  <span data-ttu-id="76c33-118">Stellen Sie sicher, dass Sie entweder den Entwicklermodus oder querladen von apps ausgewählt haben.</span><span class="sxs-lookup"><span data-stu-id="76c33-118">Be sure to either have developer mode, or sideload apps selected</span></span>

## <a name="for-linux-distro-maintainers"></a><span data-ttu-id="76c33-119">Für Linux-Distribution-Betreuer</span><span class="sxs-lookup"><span data-stu-id="76c33-119">For Linux Distro Maintainers</span></span>
<span data-ttu-id="76c33-120">Um die Veröffentlichung an den Store zu übermitteln, müssen Sie mit uns zusammenarbeiten, um die Genehmigung der Veröffentlichung zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="76c33-120">To submit to the Store, you will need to work with us to receive publishing approval.</span></span> <span data-ttu-id="76c33-121">Wenn Sie ein Linux-Verteilungs Besitzer sind, der Ihre Distribution dem Microsoft Store hinzufügen möchte, wenden Sie sich an wslpartners@microsoft.com.</span><span class="sxs-lookup"><span data-stu-id="76c33-121">If you are a Linux distribution owner interested in adding your distribution to the Microsoft Store, please contact wslpartners@microsoft.com.</span></span>

## <a name="getting-started"></a><span data-ttu-id="76c33-122">Erste Schritte</span><span class="sxs-lookup"><span data-stu-id="76c33-122">Getting Started</span></span>
<span data-ttu-id="76c33-123">Befolgen Sie die Anweisungen im [GitHub](https://github.com/Microsoft/WSL-DistroLauncher) -Repository "Distribution-Start Programm", um ein benutzerdefiniertes Linux-Distributionspaket zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="76c33-123">Follow the instructions on the [Distro Launcher GitHub repo](https://github.com/Microsoft/WSL-DistroLauncher) to create a custom Linux distro package.</span></span>

 
## <a name="team-blogs"></a><span data-ttu-id="76c33-124">Teamblogs</span><span class="sxs-lookup"><span data-stu-id="76c33-124">Team Blogs</span></span>
*  [<span data-ttu-id="76c33-125">Open Sourcing a WSL Sample for Linux Distribution Maintainer und Sideloading Custom Linux Distributionen</span><span class="sxs-lookup"><span data-stu-id="76c33-125">Open Sourcing a WSL Sample for Linux Distribution Maintainers and Sideloading Custom Linux Distributions</span></span>](https://blogs.msdn.microsoft.com/commandline/2018/03/26/wsl-distro-launcher/)
* [<span data-ttu-id="76c33-126">Befehlszeilenblog</span><span class="sxs-lookup"><span data-stu-id="76c33-126">Command-Line blog</span></span>](https://blogs.msdn.microsoft.com/commandline/)

## <a name="provide-feedback"></a><span data-ttu-id="76c33-127">Feedback bereitstellen</span><span class="sxs-lookup"><span data-stu-id="76c33-127">Provide Feedback</span></span>
* [<span data-ttu-id="76c33-128">GitHub-Repository für Distribution-Start Programm</span><span class="sxs-lookup"><span data-stu-id="76c33-128">Distro Launcher GitHub repo</span></span>](https://github.com/Microsoft/WSL-DistroLauncher)
* [<span data-ttu-id="76c33-129">GitHub Issue Tracker für WSL</span><span class="sxs-lookup"><span data-stu-id="76c33-129">GitHub issue tracker for WSL</span></span>](https://github.com/Microsoft/BashOnWindows/issues)
* [<span data-ttu-id="76c33-130">UserVoice-Befehlszeilenportal</span><span class="sxs-lookup"><span data-stu-id="76c33-130">Command-line UserVoice portal</span></span>](https://wpdev.uservoice.com/forums/266908-command-prompt-console-bash-on-ubuntu-on-windo/category/161892-bash)
