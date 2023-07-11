# Offline Razer Synapse 3 Macro module
Version / Data: Synapse (20230704), Macro(20230712, v3.8.0630.062205)

## Instructions
1. Copy `1687405298zXozYAgvRazerMacroSetup_v3.8.0630.062205.exe` into `C:\Windows\Installer\Razer Central`
    - `1687405298zXozYAgvRazerMacroSetup_v3.8.0630.062205.exe`: Macro module installer
    - `C:\Windows\Installer\Razer Central`: Space for synapse module installers
2. Run `"C:\Program Files (x86)\Razer\Synapse3\WPFUI\Framework\Razer.Synapse3.Installer\Razer.Synapse3.Installer.exe" Razer.Synapse3.Installer.exe /RazerMacro en-US True`
    - This command is to install `/RazerMacro` module into synapse 3
3. Open synapse 3 and be happy
### Note
Paths are may be different

## How did I find this method?
- I observed how the razer synapse 3 download and install modules
- Frist, it downloads installer into `C:\Windows\Installer\Razer Central` directory, with specially-crafted prefix filename.
- Second, when a user requests installation of the downloaded module, it runs a following command (for a macro module)
    - `"C:\Program Files (x86)\Razer\Synapse3\WPFUI\Framework\Razer.Synapse3.Installer\Razer.Synapse3.Installer.exe" Razer.Synapse3.Installer.exe /RazerMacro en-US True`
- I did the above process independently and it worked.