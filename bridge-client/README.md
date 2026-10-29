# DSH VS Code bridge

The browser half of the VS Code extension, packaged as a DSH web profile bundle. Install the matching VSIX in VS Code to use clipboard, link and file navigation integration. Installing this bundle alone does not add an editor to the DSH website.

The bundle declares its Host registration and browser entry through `dsh.bundle` and `dsh.client`. The release package contains compiled JavaScript and the MIT license; no credentials are included.

When the bridge appears in `dsh.profile.bundles`, the VS Code installer leaves its package and profile configuration unchanged. Upgrade or remove it through the DSH profile package manager. A mismatched extension reports that an administrator must update the bridge.

The extension's upstream connection mode supports loopback DSH services and VS Code Remote tunnels. An authenticated gateway that forbids iframe embedding requires a separate connection adapter; installing this bundle does not disable gateway login or frame protections.
