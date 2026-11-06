# DCMii F-16 Sufa Mod for DCS World

**Current version: V4.1.0** · Unofficial community project for DCS World · Made by the DCMii Modding Team (Digital Combat Mod Integration Intelligence)

**Website: [dcmii.de](https://dcmii.de)** — features, aircraft, installation guide, changelog and FAQ.

The DCMii F-16 Sufa Mod brings eight F-16 variants to DCS World, including the F-16I Sufa and the F-16D Barak, with a two-seat pilot/WSO multicrew system, native DTC support and the native AN/AAQ-33 Sniper ATP. It is based on the **IDF Mods Project** F-16 mod, which the DCMii team has overhauled, substantially extended and fixed.

> **Requirement:** DCS World with the official **DCS: F-16C Viper** module.

## Aircraft

| Variant | Seats | Notes |
| --- | --- | --- |
| F-16CM Block 50 | 1 | Integrated Center Pedestal Display (CPD) |
| F-16D Block 50 | 2 | Dorsal spine |
| F-16D Block 50 NS | 2 | No spine |
| F-16D Block 52 | 2 | Dorsal spine |
| F-16D Block 52 NS | 2 | No spine |
| F-16D Barak 30 | 2 | No rear HUD-repeater camera |
| F-16D Barak 40 | 2 | |
| F-16I Sufa | 2 | Sufa cockpit treatment and Sufa-style RWR |

## Key features

- **Multicrew:** pilot and WSO in one aircraft, synchronized cold start, Request Control (`R` in multiplayer), shared mission systems and a rear-cockpit HUD-repeater camera. In singleplayer, switch seats with `0` / `9`.
- **Native DTC:** DCS Data Transfer Cartridge support on all eight variants.
- **Native AN/AAQ-33 Sniper ATP:** selectable separately from the Litening pod, with calibrated mounting per variant.
- **Avionics and cockpit:** Sufa-style RWR, HUD/HMD rework on the two-seaters, CPD in the F-16CM.
- **Optional packages:** SPICE 2000, Python-5 and AGM-154B; CFT configurations on supported airframes.

A full overview is on [dcmii.de/features](https://dcmii.de/features).

## Download

| Option | What it is |
| --- | --- |
| **[DCMii Downloader](DCMii_F16I_Sufa_Downloader.exe)** | Recommended. Fetches the current Main and Liveries packages. Manifest-enabled: new releases are detected automatically, so you do not need a new Downloader for each update. |
| **[Google Drive](https://drive.google.com/drive/folders/1TOPeYokL09qGGidg5-iWRLYPqAdklzlh?usp=sharing)** | Direct download of the ZIP packages and the DCMii Sufa Installer. |
| **[Releases](https://github.com/DCMii-viper/DCMii/releases)** | Release history. |

**Packages**

| Package | Required | Contents |
| --- | --- | --- |
| `V4.1.0 DCMii-Project F-16 Sufa Main.zip` | Yes | `DCS_ROOT.zip` (five OvGME packages) and `SAVED_GAMES.zip` (multicrew scripts) |
| `V4.1.0 DCMii-Project F-16 Liveries.zip` | No | Israeli, Bulgarian, Hellenic and Moroccan-themed liveries |

## Installation

Disable your existing DCMii mods in OvGME before updating.

**Option A — DCMii Sufa Installer (optional).** The installer is not a standalone download of the mod. Point it at the ZIPs from the Downloader or Google Drive: it extracts the Main ZIP, places the mod packages in your selected OvGME repository, detects your Saved Games profile, installs the multicrew scripts and, if selected, the liveries. Then enable the packages in OvGME.

**Option B — Manual installation** (fully supported):

1. Extract the Main ZIP, then extract `DCS_ROOT.zip` and `SAVED_GAMES.zip` inside it.
2. Put the five package folders from `DCS_ROOT.zip` side by side into your OvGME repository (DCS-root profile).
3. Enable `DCMii-Project-F-16I_Sufa` and `DCMii-Project-F-16I Sufa PW-229 Sounds`. AGM-154B, Python-5 and SPICE 2000 are optional.
4. Merge the `Scripts` folder from `SAVED_GAMES.zip` into your active `Saved Games/DCS` profile.
5. Optional: merge the `Liveries` folder from the Liveries ZIP into the same Saved Games profile.

Step-by-step guide with folder trees: [dcmii.de/download](https://dcmii.de/download#install)

**Documentation (V4.0.0 guides — still valid for V4.1.0):**

- [Installation Instructions](V4.0.0_Installation_Instructions.pdf)
- [Beginner's Guide](V4.0.0_Beginners_Guide.pdf)
- [Feature Reference](V4.0.0_Feature_Reference.pdf)
- [V4.0.0 Changelog](V4.0.0_Changelog.pdf)

The full V4.1.0 changelog is on [dcmii.de/changelog](https://dcmii.de/changelog).

## Multiplayer

Both crew members need the same mod version, including the Saved Games scripts, and a server that supports the mod. Some servers reject modified DCS-root files through integrity checks.

**Confirmed server:** Pixel Storm — V4.1.0 is available and flyable there.

In multicrew, pilot and WSO must each request and complete rearm and refuel on their own client.

## Known issues (V4.1.0)

- Visible pilot/WSO bodies are not yet available in the dual-seat cockpits.
- Incorrect pitch or horizontal stabilizer behavior may occur during multicrew flight-control handovers.
- Singleplayer: the HUD-repeater camera may still be visible through the front cockpit seat (fixed in multiplayer).

## Community and support

- **Website:** [dcmii.de](https://dcmii.de)
- **Discord:** [discord.gg/d6KDEzaxX](https://discord.gg/d6KDEzaxX) — downloads, support tickets, release announcements
- **YouTube:** [@viper-spike](https://www.youtube.com/@viper-spike)

For support, open a ticket on Discord and include your DCS version, aircraft variant, a description of the problem and your `dcs.log` if possible.

## Credits

- **IDF Mods Project** — the original F-16I Sufa / F-16D mod and its aircraft variants
- **Kaiqi / Pobit** — Center Pedestal Display (CPD) foundation
- **Roughmaster** — Hellenic Air Force liveries
- **Crash** — Bulgarian Air Force liveries
- **DCMii Modding Team** (viper.spike) — overhaul, multicrew system, features, fixes, Downloader, Installer and packaging
- **itsTomK1** — contributions
- **Sylvi** — extensive multicrew testing
- **Pixel Storm team** — support for multiplayer development
- Everyone who submitted bug reports and feedback

This list is not exhaustive. Other original contributors keep the credit for their respective models, textures, scripts, liveries, code and tools. Existing credits, copyright notices and license information supplied with the original projects and assets must be retained. Credit for one person's work must never be assigned to someone else.

## Usage and license

Please read [LICENSE.md](LICENSE.md) before using or modifying project files. In short:

- Personal use and private modifications are permitted where the relevant rights holders allow them.
- Do not reupload, redistribute or publish this mod or modified versions without the necessary written permissions.
- Do not present this project or someone else's contributions as your own.
- Keep all existing copyright notices and creator credits intact.

Permission from one contributor does not grant rights over materials owned by other contributors.

## Disclaimer

This is an **unofficial** community modification for DCS World. It is not affiliated with or endorsed by **Eagle Dynamics**. DCS World, the DCS: F-16C Viper and all third-party content belong to their respective owners. The mod is provided as is, without warranty, to the extent permitted by law.
