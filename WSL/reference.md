---
title: 'Windows-Subsystem für Linux: Befehlsreferenz'
description: Liste der Befehle, mit denen das Windows-Subsystem für Linux verwaltet wird
keywords: BashOnWindows, bash, wsl, windows, windows subsystem for linux, windowssubsystem, ubuntu
ms.date: 07/31/2017
ms.topic: article
ms.assetid: 82908295-a6bd-483c-a995-613674c2677e
ms.custom: seodec18
ms.localizationpriority: high
ms.openlocfilehash: d74a6926fd797f2e1ede0fd5d8d080d0f1ce3f6b
ms.sourcegitcommit: 0b5a9f8982dfff07fc8df32d74d97293654f8e12
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/25/2019
ms.locfileid: "71269840"
---
# <a name="command-reference-for-windows-subsystem-for-linux"></a><span data-ttu-id="e9cb7-104">Befehlsreferenz für das Windows-Subsystem für Linux</span><span class="sxs-lookup"><span data-stu-id="e9cb7-104">Command Reference for Windows Subsystem for Linux</span></span>

<span data-ttu-id="e9cb7-105">Die beste Möglichkeit, mit dem Windows-Subsystem für Linux zu interagieren, ist die Verwendung des Befehls `wsl.exe`.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-105">The best way to interact with the Windows Subsystem for Linux is to use the `wsl.exe` command.</span></span> 


## `wsl.exe`

<span data-ttu-id="e9cb7-106">Unten finden Sie eine Liste mit allen Optionen, wenn Sie `wsl.exe` ab Windows Version 1903 verwenden.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-106">Below is a list containing all options when using `wsl.exe` as of Windows Version 1903.</span></span>

<span data-ttu-id="e9cb7-107">Syntax: `wsl [Argument] [Options...] [CommandLine]`</span><span class="sxs-lookup"><span data-stu-id="e9cb7-107">Using: `wsl [Argument] [Options...] [CommandLine]`</span></span>

### <a name="arguments-for-running-linux-binaries"></a><span data-ttu-id="e9cb7-108">Argumente für das Ausführen von Linux-Binärdateien</span><span class="sxs-lookup"><span data-stu-id="e9cb7-108">Arguments for running Linux binaries</span></span>

* <span data-ttu-id="e9cb7-109">**Ohne Argumente**</span><span class="sxs-lookup"><span data-stu-id="e9cb7-109">**Without arguments**</span></span>

  <span data-ttu-id="e9cb7-110">Wenn keine Befehlszeile angegeben wird, startet „wsl.exe“ die Standardshell.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-110">If no command line is provided, wsl.exe launches the default shell.</span></span>

* <span data-ttu-id="e9cb7-111">**--exec, -e \<BefehlsZeile>**</span><span class="sxs-lookup"><span data-stu-id="e9cb7-111">**--exec, -e \<CommandLine>**</span></span>
  
  <span data-ttu-id="e9cb7-112">Führt den angegebenen Befehl ohne Verwendung der Linux-Standardshell aus.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-112">Execute the specified command without using the default Linux shell.</span></span>

* **--**
  
  <span data-ttu-id="e9cb7-113">Übergibt die verbleibende Befehlszeile unverändert.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-113">Pass the remaining command line as is.</span></span>

<span data-ttu-id="e9cb7-114">Die oben genannten Befehle akzeptieren außerdem die folgenden Optionen:</span><span class="sxs-lookup"><span data-stu-id="e9cb7-114">The above commands also accept the following options:</span></span>

* <span data-ttu-id="e9cb7-115">**--distribution, -d \<Distribution>**</span><span class="sxs-lookup"><span data-stu-id="e9cb7-115">**--distribution, -d \<Distro>**</span></span>

  <span data-ttu-id="e9cb7-116">Führt die angegebene Distribution aus.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-116">Run the specified distribution.</span></span>

* <span data-ttu-id="e9cb7-117">**--user, -u \<BenutzerName>**</span><span class="sxs-lookup"><span data-stu-id="e9cb7-117">**--user, -u \<UserName>**</span></span>

  <span data-ttu-id="e9cb7-118">Ausführung als der angegebene Benutzer.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-118">Run as the specified user.</span></span>

### <a name="arguments-for-managing-windows-subsystem-for-linux"></a><span data-ttu-id="e9cb7-119">Argumente für die Verwaltung des Windows-Subsystems für Linux</span><span class="sxs-lookup"><span data-stu-id="e9cb7-119">Arguments for managing Windows Subsystem for Linux</span></span>

* <span data-ttu-id="e9cb7-120">**--export \<Distribution> \<DateiName>**</span><span class="sxs-lookup"><span data-stu-id="e9cb7-120">**--export \<Distro> \<FileName>**</span></span>
  
  <span data-ttu-id="e9cb7-121">Exportiert die Distribution in eine TAR-Datei.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-121">Exports the distribution to a tar file.</span></span> <span data-ttu-id="e9cb7-122">Der Dateiname kann „-“ für Standardausgabe sein.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-122">The filename can be - for standard output.</span></span>

* <span data-ttu-id="e9cb7-123">**--import \<Distribution> \<InstallationsOrt> \<DateiName>**</span><span class="sxs-lookup"><span data-stu-id="e9cb7-123">**--import \<Distro> \<InstallLocation> \<FileName>**</span></span>
  
  <span data-ttu-id="e9cb7-124">Importiert die angegebene TAR-Datei als neue Distribution.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-124">Imports the specified tar file as a new distribution.</span></span> <span data-ttu-id="e9cb7-125">Der Dateiname kann „-“ für Standardeingabe sein.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-125">The filename can be - for standard input.</span></span>

* <span data-ttu-id="e9cb7-126">**--list, -l [Optionen]**</span><span class="sxs-lookup"><span data-stu-id="e9cb7-126">**--list, -l [Options]**</span></span>
  
  <span data-ttu-id="e9cb7-127">Listet Distributionen auf.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-127">Lists distributions.</span></span>

  <span data-ttu-id="e9cb7-128">Optionen:</span><span class="sxs-lookup"><span data-stu-id="e9cb7-128">Options:</span></span>
  * <span data-ttu-id="e9cb7-129">**--all**</span><span class="sxs-lookup"><span data-stu-id="e9cb7-129">**--all**</span></span>
      
    <span data-ttu-id="e9cb7-130">Listet alle Distributionen auf, einschließlich Distributionen, die zurzeit installiert oder deinstalliert werden.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-130">List all distributions, including distributions that are currently being installed or uninstalled.</span></span>

  * <span data-ttu-id="e9cb7-131">**--running**</span><span class="sxs-lookup"><span data-stu-id="e9cb7-131">**--running**</span></span>
      
    <span data-ttu-id="e9cb7-132">Listet nur Distributionen auf, die zurzeit ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-132">List only distributions that are currently running.</span></span>

* <span data-ttu-id="e9cb7-133">**--set-default, -s \<Distribution>**</span><span class="sxs-lookup"><span data-stu-id="e9cb7-133">**--set-default, -s \<Distro>**</span></span>
  
  <span data-ttu-id="e9cb7-134">Legt die Distribution als Standard fest.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-134">Sets the distribution as the default.</span></span>

* <span data-ttu-id="e9cb7-135">**--terminate, -t \<Distribution>**</span><span class="sxs-lookup"><span data-stu-id="e9cb7-135">**--terminate, -t \<Distro>**</span></span>
  
  <span data-ttu-id="e9cb7-136">Beendet die angegebene Distribution.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-136">Terminates the specified distribution.</span></span>

* <span data-ttu-id="e9cb7-137">**--unregister \<Distribution>**</span><span class="sxs-lookup"><span data-stu-id="e9cb7-137">**--unregister \<Distro>**</span></span>
  
  <span data-ttu-id="e9cb7-138">Hebt die Registrierung der Distribution auf.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-138">Unregisters the distribution.</span></span>
   
* <span data-ttu-id="e9cb7-139">**--help**: Zeigt Syntaxinformationen an.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-139">**--help** Display usage information.</span></span>

## <a name="additional-commands"></a><span data-ttu-id="e9cb7-140">Weitere Befehle</span><span class="sxs-lookup"><span data-stu-id="e9cb7-140">Additional Commands</span></span>

<span data-ttu-id="e9cb7-141">Es gibt auch historische Befehle für die Interaktion mit dem Windows-Subsystem für Linux.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-141">There are also historic commands to interact with the Windows Subsystem for Linux.</span></span> <span data-ttu-id="e9cb7-142">Ihre Funktionalität ist in `wsl.exe` enthalten, sie sind jedoch weiterhin zur Verwendung verfügbar.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-142">Their functionality is encompassed within `wsl.exe`, but they are still available for use.</span></span> 

### `wslconfig.exe`

<span data-ttu-id="e9cb7-143">Mit diesem Befehl können Sie Ihre WSL-Distribution konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-143">This command lets you configure your WSL distribution.</span></span> <span data-ttu-id="e9cb7-144">Es folgt eine Liste der zugehörigen Optionen.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-144">Below is a list of its options.</span></span>

<span data-ttu-id="e9cb7-145">Syntax: `wslconfig [Argument] [Options...]`</span><span class="sxs-lookup"><span data-stu-id="e9cb7-145">Using: `wslconfig [Argument] [Options...]`</span></span>

#### <a name="arguments"></a><span data-ttu-id="e9cb7-146">Argumente</span><span class="sxs-lookup"><span data-stu-id="e9cb7-146">Arguments</span></span>
* <span data-ttu-id="e9cb7-147">**/l, /list [Optionen]**</span><span class="sxs-lookup"><span data-stu-id="e9cb7-147">**/l, /list [Options]**</span></span>
  
  <span data-ttu-id="e9cb7-148">Listet registrierte Distributionen auf.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-148">Lists registered distributions.</span></span>
  
  <span data-ttu-id="e9cb7-149">Optionen:</span><span class="sxs-lookup"><span data-stu-id="e9cb7-149">Options:</span></span>
    * <span data-ttu-id="e9cb7-150">**/all**</span><span class="sxs-lookup"><span data-stu-id="e9cb7-150">**/all**</span></span>
    
      <span data-ttu-id="e9cb7-151">Listet optional alle Distributionen auf, einschließlich Distributionen, die zurzeit installiert oder deinstalliert werden.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-151">Optionally list all distributions, including distributions that are currently being installed or uninstalled.</span></span>

    * <span data-ttu-id="e9cb7-152">**/running**</span><span class="sxs-lookup"><span data-stu-id="e9cb7-152">**/running**</span></span>
      
      <span data-ttu-id="e9cb7-153">Listet nur Distributionen auf, die zurzeit ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-153">List only distributions that are currently running.</span></span>

* <span data-ttu-id="e9cb7-154">**/s, /setdefault \<Distribution>**</span><span class="sxs-lookup"><span data-stu-id="e9cb7-154">**/s, /setdefault \<Distro>**</span></span>
  
  <span data-ttu-id="e9cb7-155">Legt die Distribution als Standard fest.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-155">Sets the distribution as the default.</span></span>

* <span data-ttu-id="e9cb7-156">**/t, /terminate \<Distribution>**</span><span class="sxs-lookup"><span data-stu-id="e9cb7-156">**/t, /terminate \<Distro>**</span></span>
  
  <span data-ttu-id="e9cb7-157">Beendet die Distribution.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-157">Terminates the distribution.</span></span>

* <span data-ttu-id="e9cb7-158">**/u, /unregister \<Distribution>**</span><span class="sxs-lookup"><span data-stu-id="e9cb7-158">**/u, /unregister \<Distro>**</span></span>
  
  <span data-ttu-id="e9cb7-159">Hebt die Registrierung der Distribution auf.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-159">Unregisters the distribution.</span></span>
   
* <span data-ttu-id="e9cb7-160">**/upgrade \<Distribution>**</span><span class="sxs-lookup"><span data-stu-id="e9cb7-160">**/upgrade \<Distro>**</span></span>
  
  <span data-ttu-id="e9cb7-161">Führt ein Upgrade der Distribution auf das WslFs-Dateisystemformat durch.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-161">Upgrades the distribution to the WslFs file system format.</span></span>

### `bash.exe`

<span data-ttu-id="e9cb7-162">Dieser Befehl wird verwendet, um eine Bash-Shell zu starten.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-162">This command is used to start a bash shell.</span></span> <span data-ttu-id="e9cb7-163">Unten finden Sie die Optionen, die Sie mit diesem Befehl verwenden können.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-163">Below are the options you can use with this command.</span></span>

<span data-ttu-id="e9cb7-164">Syntax: `bash [Options...]`</span><span class="sxs-lookup"><span data-stu-id="e9cb7-164">Using: `bash [Options...]`</span></span>

* <span data-ttu-id="e9cb7-165">**Keine Option angegeben**</span><span class="sxs-lookup"><span data-stu-id="e9cb7-165">**No Option given**</span></span>
  
  <span data-ttu-id="e9cb7-166">Startet die Bash-Shell im aktuellen Verzeichnis.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-166">Launches the Bash shell in the current directory.</span></span> <span data-ttu-id="e9cb7-167">Wenn die Bash-Shell nicht installiert ist, wird automatisch `lxrun /install` ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-167">If the Bash shell is not installed automatically runs `lxrun /install`</span></span>

* **~**
  
  <span data-ttu-id="e9cb7-168">`bash ~` startet die Bash-Shell im Basisverzeichnis des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-168">`bash ~` launches the bash shell into the user's home directory.</span></span>  <span data-ttu-id="e9cb7-169">Vergleichbar mit der Ausführung von `cd ~`.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-169">Similar to running `cd ~`.</span></span>

* <span data-ttu-id="e9cb7-170">**-c "\<Befehl>"**</span><span class="sxs-lookup"><span data-stu-id="e9cb7-170">**-c "\<command>"**</span></span>
  
  <span data-ttu-id="e9cb7-171">Führt den Befehl aus, gibt die Ausgabe aus, und kehrt zur Windows-Eingabeaufforderung zurück.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-171">Runs the command, prints the output and exits back to the Windows command prompt.</span></span>
    
  <span data-ttu-id="e9cb7-172">Beispiel: `bash -c "ls"`.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-172">Example:  `bash -c "ls"`.</span></span>

## <a name="deprecated-commands"></a><span data-ttu-id="e9cb7-173">Veraltete Befehle</span><span class="sxs-lookup"><span data-stu-id="e9cb7-173">Deprecated Commands</span></span>

<span data-ttu-id="e9cb7-174">`lxrun.exe` war der erste Befehl, der zum Installieren und Verwalten des Windows-Subsystems für Linux verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-174">The `lxrun.exe` was the first command used to install and manage the Windows Subsystem for Linux.</span></span> <span data-ttu-id="e9cb7-175">Er gilt ab Windows 10 Version 1803 und höher als veraltet.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-175">It is deprecated as of Windows 10 1803 and later.</span></span>

<span data-ttu-id="e9cb7-176">Der Befehl `lxrun.exe` kann verwendet werden, um direkt mit dem [Windows-Subsystem für Linux (WSL)](https://msdn.microsoft.com/en-us/commandline/wsl/faq#what-windows-subsystem-for-linux-wsl-) zu interagieren.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-176">The command `lxrun.exe` can be used to interact with the [Windows Subsystem for Linux (WSL)](https://msdn.microsoft.com/en-us/commandline/wsl/faq#what-windows-subsystem-for-linux-wsl-) directly.</span></span>  <span data-ttu-id="e9cb7-177">Diese Befehle werden im Verzeichnis `\Windows\System32` installiert und können in einer Windows-Eingabeaufforderung oder in PowerShell ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-177">These commands are installed into the `\Windows\System32` directory and may be run within a Windows command prompt or in PowerShell.</span></span>

| <span data-ttu-id="e9cb7-178">Befehl</span><span class="sxs-lookup"><span data-stu-id="e9cb7-178">Command</span></span>                     | <span data-ttu-id="e9cb7-179">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e9cb7-179">Description</span></span>                     |
|:----------------------------|:---------------------------|
| `lxrun`                     | <span data-ttu-id="e9cb7-180">Der lxrun-Befehl wird verwendet, um die WSL-Instanz zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-180">The lxrun command is used to manage the WSL instance.</span></span> |
| `lxrun /install`            | <span data-ttu-id="e9cb7-181">Startet den Download- und Installationsvorgang.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-181">Starts the download and install process.</span></span> <br/> <span data-ttu-id="e9cb7-182">**/y** kann hinzugefügt werden, um alle Eingabeaufforderungen zu umgehen.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-182">**/y** may be added to bypass all prompts.</span></span>  <span data-ttu-id="e9cb7-183">Die Bestätigungsaufforderung wird automatisch akzeptiert, und der Standardbenutzer wird auf „root“ festgelegt.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-183">The confirmation prompt is automatically accepted and the default user is set to root.</span></span>          |
| `lxrun /uninstall`          | <span data-ttu-id="e9cb7-184">Deinstalliert und löscht das Ubuntu-Image.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-184">Uninstalls and deletes the Ubuntu image.</span></span>  <span data-ttu-id="e9cb7-185">Standardmäßig wird hierdurch nicht das Ubuntu-Basisverzeichnis des Benutzers entfernt.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-185">By default this does not remove the user's Ubuntu home directory.</span></span> <br/> <span data-ttu-id="e9cb7-186">**/y** kann hinzugefügt werden, um die Bestätigungsaufforderung automatisch zu akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-186">**/y** may be added to automatically accept the confirmation prompt</span></span> <br/><span data-ttu-id="e9cb7-187">**/full** deinstalliert und löscht das Ubuntu-Basisverzeichnis des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-187">**/full** uninstalls and deletes the user's Ubuntu home directory</span></span>         |
| `lxrun /setdefaultuser <userName>`     | <span data-ttu-id="e9cb7-188">Legt die Standard-Bash für den Ubuntu-Benutzer fest.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-188">Sets the default Bash on Ubuntu user.</span></span> <span data-ttu-id="e9cb7-189">Fordert zur Eingabe eines Kennworts auf, wenn der angegebene Benutzer nicht vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-189">Will prompt for a password if the specified user does not exist.</span></span>  <span data-ttu-id="e9cb7-190">Weitere Informationen finden Sie unter https://aka.ms/wslusers.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-190">For more information visit: https://aka.ms/wslusers.</span></span> <br/> <span data-ttu-id="e9cb7-191">**/y** umgeht die Eingabeaufforderung für das Kennwort.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-191">**/y** Bypasses promping for the password.</span></span>  <span data-ttu-id="e9cb7-192">Der Benutzer wird ohne Kennwort erstellt.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-192">The user will be created without a password.</span></span>|
| `lxrun /update`            | <span data-ttu-id="e9cb7-193">Aktualisiert den Paketindex des Subsystems.</span><span class="sxs-lookup"><span data-stu-id="e9cb7-193">Updates the subsystem's package index</span></span>          |
