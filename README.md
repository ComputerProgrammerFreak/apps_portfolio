# Software Application Portfolio by Aiden Halm
A portfolio of software I've developed in my spare time and a couple from team projects at UTAS.

# Current Large Projects
## 2022 – Account Manager
Development started in 2022 using Dart/Flutter and Google Firebase.

![account_manager.png](/images/account_manager.png)
(work in progress...)

#### Motivation
While there are many solutions already available, I am very curious about how they are created, which is why I decided to start building my own account manager.
#### Features
Account addition, removal, and modification of details such as organisation, email, name, password, security questions, and tags.
Encryption:
* The data is stored using AES-256 encryption.
* RSA-2048 encryption is used to share the encryption keys when setting up a new device. Ideally, the new device would then generate a new data encryption key from the received master key, for now though it just copies the keys.
Appearance settings page for:
* Primary and Accent colours
* Theme mode: Light, Dark, System
* Dialog Theme
	* Use bevelled corners
	* Border visibility
	* Border colour

Encryption page for distributing, deleting, or regenerating keys.

# Current Medium Projects
## 2025 – Dualtron City Utilities / eScooter Utilities
Development started in 2025 using Dart/Flutter.

Personal use eScooter utility application for tracking trips, statistics display, and a couple calculators.

Screenshots (work in progress):

![charge_calculator.png](/images/eScooter_utilities/charging_calculator.png)
![trip_calculator.png](/images/eScooter_utilities/trip_calculator.png)

# Current Small Projects
## 2025 – Secure Share
Development started in 2024 using Dart/Flutter.

![secure_share_home.png](/images/secure_share_home.png)

![secure_share_receive.png](/images/secure_share_receive.png)
###### \*Swanky PC and it’s IP address is just an example.

#### Motivation
I often require sending text from one device to another. I made this application to allow me to send text to another device in an end-to-end encrypted manner using RSA-2048 encryption.
#### Features
* Share via Local Area Network
* Share via QR Code (work in progress)
* Share text
* Share files (work in progress)
* Ability to save and manage recent devices

## 2024 – Code Counter
Development started in 2024 using Dart/Flutter (based upon my 2018 implementation in C#).

![code_counter.png](/images/code_counter.png)

#### Motivation
During development, I sometimes like to assess the size of my projects. While I initially used scripts to perform this task, I decided to streamline the process by developing this tool as a more informative alternative.
#### Features
Overview of all projects showing file count, size, lines of code (LOC), and total lines. There is also a counter for LOC across all projects.
Per project:
* Total file count, LOC, and lines.
* Button to highlight file with largest LOC.
* Left panel for folder hierarchy.
* Right panel for file and subfolder display.
	* Displays file info such as file size and LOC.

# Past Large Projects
## 2023 – UTAS KIT318 Project: Weather Service (Cloud Computing)
Developed in 2023 using Java, Nectar Cloud Platform, and OpenStack4j.
My team’s assignment was to create a cloud-based distributed computing application (PaaS) to analyse given weather data. The program provides the following functionalities:
* Compute average monthly min/max temperature from year and station ID.
* Compute average yearly min/max temperature of all stations from year.
* Find the month with the highest/lowest temperature from year and station ID.

When the client starts, they can either login using their Unique User ID (UUID) or create a new account. Then they’re presented with the following options:
1.	Create a Job
2.	Cancel a Job
3.	Print Job Progress
4.	Logout

Technical implementation:
* **Architecture**: Our program used a client-server model using asynchronous sockets, where each client sends commands to the server to create jobs, query job progress, or cancel jobs.
* **Cloud Integration**: OpenStack4j was used to remotely access and control the VMs. For example, waking them to start a new job, or pausing the VM.
* **Code Base**: Our project consisted of 5,331 lines of code.
My role in this project was implementing the client-server framework, command handling, user account management, worker allocation and management, and the text-based user interface.

![utas_kit318_project_weather_service.png](/images/utas_kit318_project_weather_service.png)

# Past Small Projects
## 2024 – Watch_Dogs Session Tool
Developed in 2024 using C# and .NET Framework.

![watch_dogs_session_tool.png](/images/watch_dogs_session_tool.png)

#### Motivation
A very simple tool to initiate a session migration if hackers/griefers join the lobby and start interfering with my missions.
#### Features
To minimise disruption, the tool has shortcut activation and auto-switching back to the game.

## 2024 – eScooter Gear Calculator
Development started in 2024 using Dart/Flutter.

**Notice:**
> This project has been deprecated in favour of the newer remake "eScooter Utilities".

#### Motivation
Calculating the speed limit percentage for a desired speed and gear is easy but tedious. So I have developed this simple calculator to do the work for me.
#### Limitations
It’s hard coded with the gear ratios of my eScooter thus not useful for other models.
#### Future Development Plans
I plan to implement the ability to add new eScooter models with their required data such as gear ratios and max speed. This will need an eScooter management screen for adding and removing models.
The project will be expanded to calculate charging information as well based on current voltage and average voltage charge per hour. For that, a trip logger will also be implemented to track distances and power usage.

## 2023 – UTAS KIT325 Project: The Kings Guard (Basic Malware Scanner)
Developed in 2023 using C# and .NET Framework

For this assignment, our team chose to develop a basic malware scanner, using signature-based detection with MD5/TLSH. My contributions involved developing the scanning UI, toast notifications, USB detection, and malware analysis components.

![utas_kit325_project_the_kings_guard.png](/images/utas_kit325_project_the_kings_guard.png)

## 2022 – Symbolic Linker
Developed in 2022 Feb using C# and .NET Framework.
#### Motivation
Some applications are installed on the main drive with no option to change it. After moving the data, this tool allows me to create a link in the original location pointing to the new location without affecting any app installations.
#### Use Case
Moving large applications and data caches from smaller hard drives to larger capacity drives while preserving the installation.
#### Future Development Plans
The ability to move a folder and create a symbolic link in the original location. This removes the need to move the folder manually first.

## 2022 – Visual Studio Project Backup
Developed in 2022 using C# / .NET Framework, Microsoft.Build.Framework, and WinRAR (must be installed).

![visual_studio_project_backup.png](/images/visual_studio_project_backup.png)

#### Motivation and Use Case
When I discovered my consistent process for creating backups for my C# Visual Studio projects, I made this tool to automate it. The tool excludes data to reduce file size such as intermediatory and resulting build files. It also uses the backup filename format “project_name – [yyyy-MM-dd_THH.mm.ss]”.
#### Improvements
I may introduce custom name formats instead of using the hard-coded one.

## 2022 – Image to Icon
Developed in 2022 using C# and .NET Framework.

![image_to_icon.png](/images/image_to_icon.png)

#### Motivation
I developed this simple tool to quickly convert images into icon files for various use cases such as creating app icons.

## 2021 – Mass File Rename Utility
Developed in 2021 using C# and .NET Framework.

![mass_file_rename_utility.png](/images/mass_file_rename_utility.png)

#### Motivation
I found myself renaming lots of files with similar naming formats, most commonly removing some trailing prefix like "- YouTube" to URL files or downloaded music with album info in the file name. This tool allows me to rename many files at once with a new name format.
#### Features
*	Filename case modification: Unchanged, Uppercase, Lowercase, Sentence, or Title Case
*	Filename modification: Append, Prepend, Truncate Start. Truncate End, Replace Text

## 2021 – GTAV Online Lobby Tool
Developed in 2021 using C# and .NET Framework.

![gtav_online_lobby_tool.png](/images/gtav_online_lobby_tool.png)

#### Motivation
A very simple tool to initiate a session migration if hackers join the lobby and start bullying players or interfering with my critical missions.
#### Features
To minimise disruption, the tool has shortcut activation and auto-switching back to the game.
