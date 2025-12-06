# SkyrimLovense ([Nexus Mods Mirror](https://www.nexusmods.com/skyrimspecialedition/mods/133698))

Lovense API for TES5 Skyrim, which allows authors to control connetected Lovense Toys through Papyrus Scripts.  
Connection is done through either the cnosole or a custom user interface, the code for which can be viewed [here](https://github.com/KrisV-777/Skyrim-Lovense-UI). Instructions are found on the [Nexus Page](https://www.nexusmods.com/skyrimspecialedition/mods/133698).

Usage instructions for users can be found on the [Nexus Page](https://www.nexusmods.com/skyrimspecialedition/mods/133698).  
The Papyrus API, which includes all documentation, can be found [here](https://github.com/KrisV-777/Skyrim-Lovense/blob/main/dist/Source/Scripts/Lovense.psc).

## Requirements
* [xmake](https://xmake.io/#/)
	* Add this to your `PATH`
* [PowerShell](https://github.com/PowerShell/PowerShell/releases/latest)
* [Visual Studio Community 2022](https://visualstudio.microsoft.com/)
	* Desktop development with C++
* [CommonLibSSE](https://github.com/alandtse/CommonLibVR/tree/ng)
	* You need to build from the alandtse/ng branch
* Create Environment Variables:
  * `XSE_TES5_MODS_PATH`: Path to your MO2/Vortex `mods` folder

## Building
```
git clone https://github.com/KrisV-777/Skyrim-Lovense.git
cd Skyrim-Lovense
git submodule update --init --recursive
xmake f -m release [
	--copy_to_papyrus=(y/n)		# build & create/update the "SkyrimLovense" papyrus mod instance
]
xmake
```
