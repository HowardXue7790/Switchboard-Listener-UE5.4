# UE 5.4 Standalone Switchboard Package

This repository provides a standalone package for running UE 5.4 Switchboard and Switchboard Listener without requiring a full Unreal Engine installation.

Chinese version: [README.md](README.md)

## Contents

- `StartSwitchboard.bat`: Starts Switchboard.
- `StartSwitchboardListener.bat`: Starts Switchboard Listener.
- `Engine/`: UE 5.4 files required by Switchboard.

## Quick Start

1. Download or clone this repository.
2. Double-click `StartSwitchboard.bat` to start Switchboard.
3. Double-click `StartSwitchboardListener.bat` to start Switchboard Listener.

## First Launch Notes

On the first Switchboard launch, the application creates a Python virtual environment in:

```text
.\Engine\Extras\ThirdPartyNotUE\SwitchboardThirdParty\Python
```

After the virtual environment is created, the following script contains absolute paths for the current machine:

```text
.\Engine\Extras\ThirdPartyNotUE\SwitchboardThirdParty\Python\Scripts\activate.bat
```

## Moving to Another Computer

If you copy this repository to another computer, delete the following directory before starting Switchboard on the new machine:

```text
.\Engine\Extras\ThirdPartyNotUE\SwitchboardThirdParty\Python
```

Switchboard will recreate the Python virtual environment on the new computer, which prevents startup issues caused by absolute paths from the previous machine.

## Requirements

- Windows
- UE 5.4 Switchboard runtime files included in this repository
