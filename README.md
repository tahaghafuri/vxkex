# Development
I stopped development of this version and am developing https://github.com/vxkex/vxkex/.

# VxKex - Run Modern Windows Apps on Windows 7

VxKex provides API extensions that enable Windows 8, 8.1, and 10-exclusive applications to run on Windows 7.

## Quick Start

1. Install VxKex
2. Right-click any program (.exe or .msi)
3. Open Properties
4. Select the VxKex tab
5. Check "Enable VxKex for this program"
6. Run the program

![VxKex configuration GUI](/screenshot.png)

> For advanced configuration, refer to **"Application Compatibility List.docx"** in `C:\Program Files\VxKex`

## Features

- No system file modifications
- Minimal system impact
- No background services
- Optional shell extensions

## Supported Applications

Notable applications that work with VxKex include:

- Modern browsers (Firefox, Chromium, Opera)
- Development tools (VSCode, Qt Creator, Python, Zig)
- Media applications (MPV, GIMP, Blender)
- Popular apps (Discord Canary, Spotify, GitHub Desktop)

> Full compatibility list available in the installed documentation

## Requirements

- Windows 7 Service Pack 1
- Recommended updates:
    - KB2533623
    - KB2670838
- Compatible with Extended Security Updates (ESUs)

## FAQ

#### Q: Does it work with games?
A: Currently limited support. Future releases may improve gaming compatibility.

#### Q: Does it work on Windows 8/8.1?
A: VxKex is designed exclusively for Windows 7.

#### Q: How does it work?
A: VxKex injects a DLL using IFEO registry keys and redirects API calls to compatible implementations.

## Technical Details

VxKex uses:
- IFEO (Image File Execution Options) for DLL injection
- Import table modification for API redirection
- Custom DLL implementations of modern Windows APIs
