# Windows Developer Setup Scripts

[![🇯🇵 日本語](https://img.shields.io/badge/%F0%9F%87%AF%F0%9F%87%B5-日本語-white)](./README.ja.md) [![🇺🇸 English](https://img.shields.io/badge/%F0%9F%87%BA%F0%9F%87%B8-English-white)](./README.md)

PowerShell scripts for automating Windows developer environment setup. Quickly install essential development tools with a single script.

## Included Software

This script automatically downloads and installs the following software:

1. **Git** - Version control system
2. **TortoiseGit** - Windows Shell Interface to Git
3. **Google Chrome** - Web browser
4. **WinMerge** - Differencing and merging tool
5. **Visual Studio Code** - Code editor
6. **Sakura Editor** - Text editor (Japanese)
7. **Winshot** - Screenshot tool

## Prerequisites

- Windows 10/11
- PowerShell 5.1 or higher
- Administrator privileges

## Usage

1. Save the script as `setup-dev-environment.ps1`
2. Open PowerShell as Administrator
3. Allow script execution by running:
   ```powershell
   Set-ExecutionPolicy -ExecutionPolicy Bypass -Scope Process
   ```
4. Navigate to the directory containing the script
5. Run the script:
   ```powershell
   .\setup-dev-environment.ps1
   ```

## Installation Details

- Standard installer-based software (Git, TortoiseGit, Chrome, WinMerge, VSCode, Sakura Editor) will be installed to their default locations.
- ZIP-based software (Winshot) will be extracted to `C:\tools\[SoftwareName]`.

## Customization

You can modify the script to:
- Change software versions by updating download URLs
- Add or remove software items
- Customize installation parameters
- Change installation directories

## License

MIT

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.
