# DCMii F-16 Sufa Mod for DCS World

**Current version: V4.2.0** · Unofficial community project for DCS World · Made by the DCMii Modding Team (Digital Combat Mod Integration Intelligence)

**Website: [dcmii.de](https://dcmii.de)** — features, aircraft, installation guide, changelog and FAQ.

The DCMii F-16 Sufa Mod brings eight F-16 variants to DCS World, including the F-16I Sufa and the F-16D Barak, with a two-seat pilot/WSO multicrew system, visible crew figures, native DTC support, the native AN/AAQ-33 Sniper ATP and the GBU-39/53 Small Diameter Bombs. It is based on the **IDF Mods Project** F-16 mod, which the DCMii team has overhauled, substantially extended and fixed.

> **Requirement:** DCS World with the official **DCS: F-16C Viper** module.

## What's new in V4.2.0

- **Pilot and WSO figures** in every two-seat cockpit. They follow stick, throttle and rudder pedals; your own head is hidden. Show or hide them with `RShift+P`.
- **Leg kneeboard** that shows and follows the current kneeboard page, with a DCMii start page and support for your own pages.
- **Small Diameter Bombs:** GBU-39 SDB and GBU-53/B SDB II on BRU-61 racks (1 to 4 bombs) at stations 3 and 7 on all eight variants, with SMS page support.
- **HSD moving map:** PICT mode shows a live map beneath the HSD symbology.
- **Night operations:** NVG and JHMCS at the same time, a white-phosphor night-vision image and a clearer targeting-pod FLIR picture.
- **Realistic two-seat fuel**, corrected CFT and tank weights, and a DTC that accepts cartridges of the DCMii aircraft types.
- **New optional package: Modern AMRAAM** (AIM-120D3 and AIM-120C8).
- More working controls in the two-seaters, a full-travel throttle lever, new main menu and loading screens, and the **Server Edition 4.2** for dedicated servers.

Full details: [V4.2.0 Changelog](V4.2.0_Changelog.pdf) (covers all changes since V4.0.0) · [dcmii.de/changelog](https://dcmii.de/changelog)

## Aircraft

| Variant | Seats | Notes |
| --- | --- | --- |
| F-16CM Block 50 | 1 | Integrated Center Pedestal Display (CPD) |
| F-16D Block 50 | 2 | Dorsal spine, pilot and WSO figures |
| F-16D Block 50 NS | 2 | No spine, pilot and WSO figures |
| F-16D Block 52 | 2 | Dorsal spine, pilot and WSO figures |
| F-16D Block 52 NS | 2 | No spine, pilot and WSO figures |
| F-16D Barak 30 | 2 | Pilot and WSO figures; no rear HUD-repeater camera |
| F-16D Barak 40 | 2 | Pilot and WSO figures |
| F-16I Sufa | 2 | Sufa cockpit treatment, Sufa-style RWR, pilot and WSO figures |

## Key features

- **Multicrew:** pilot and WSO in one aircraft, synchronized cold start, Request Control (`R` in multiplayer), shared mission systems and a rear-cockpit HUD-repeater camera.
- **Native DTC:** DCS Data Transfer Cartridge support on all eight variants.
- **Native AN/AAQ-33 Sniper ATP:** selectable separately from the Litening pod, with calibrated mounting per variant.
- **Avionics and cockpit:** Sufa-style RWR, HSD moving map, HUD/HMD rework on the two-seaters, CPD in the F-16CM.
- **Weapons:** GBU-39/53 on all variants; optional Modern AMRAAM, SPICE 2000, Python-5 and AGM-154B packages; CFT configurations on supported airframes.

### Controls

| Key | Function |
| --- | --- |
| `9` / `0` | Singleplayer: select the pilot (`9`) or WSO (`0`) seat |
| `R` | Multiplayer: request flight control without changing seats |
| `RShift+P` | Show or hide the pilot and WSO figures |

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
| `V4.2.0 DCMii-Project F-16 Sufa Main.zip` | Yes | `DCS_ROOT.zip` (six OvGME packages) and `SAVED_GAMES.zip` (multicrew scripts: `DCMII_MC_V3` and `Hooks`) |
| `V4.2.0 DCMii-Project F-16 Liveries.zip` | No | `F-16C_50` (6 single-seat liveries) and `F-16D_50` (2 dual-seat liveries) |

A separate **Server Edition 4.2** is available for dedicated servers: aircraft, loadouts including GBU-39/53, fuel, DTC and models. Use it with a matching client build.

## Installation

Close DCS and disable your existing DCMii mods in OvGME before updating. Replace old DCMii package folders completely instead of merging new files into them.

**Option A — DCMii Sufa Installer (optional).** The installer is not a standalone download of the mod. Point it at the ZIPs from the Downloader or Google Drive: it extracts the Main ZIP, places the mod packages in your selected OvGME repository, detects your Saved Games profile, installs the multicrew scripts and, if selected, the liveries. Then enable the packages in OvGME.

**Option B — Manual installation** (fully supported):

1. Extract the Main ZIP, then extract `DCS_ROOT.zip` and `SAVED_GAMES.zip` inside it. Do not drop the outer Main ZIP into DCS.
2. Put the six package folders from `DCS_ROOT.zip` side by side into your OvGME repository (DCS-root profile). Do not merge them together.
   ```
   DCS-Mods/   (example OvGME repository)
   ├── DCMii-Project-F-16I_Sufa                required
   ├── DCMii-Project-F-16I Sufa PW-229 Sounds  required
   ├── DCMii-Project-Modern-AMRAAM             optional
   ├── DCMii-Project-AGM-154B                  optional
   ├── DCMii-Project-Python-5                  optional
   └── DCMii-Project-Spice_2000                optional
   ```
3. With DCS closed, enable `F-16I_Sufa` and `PW-229 Sounds` in OvGME, plus any optional packages you want. Enable SPICE 2000 after the main package.
4. `SAVED_GAMES.zip` holds the folders `DCMII_MC_V3` and `Hooks` **without** a `Scripts` folder around them. Extract both into `Saved Games/DCS/Scripts` of the profile your DCS actually uses (for example `DCS` or `DCS.openbeta`). Create `Scripts` if it does not exist; merge into an existing `Hooks` folder and replace old DCMii files when asked.
   ```
   Saved Games/DCS/Scripts/
   ├── DCMII_MC_V3/        multicrew transport
   └── Hooks/
       └── DCMII_MC_Role.lua
   ```
5. Optional: extract the Liveries ZIP into `Saved Games/DCS/Liveries`. It contains the folders `F-16C_50` and `F-16D_50` directly.

Step-by-step guide with folder trees: [dcmii.de/download](https://dcmii.de/download#install)

**Documentation (V4.2.0):**

- [Installation Instructions](V4.2.0_Installation_Instructions.pdf)
- [Beginner's Guide](V4.2.0_Beginners_Guide.pdf)
- [Feature Reference](V4.2.0_Feature_Reference.pdf)
- [Changelog](V4.2.0_Changelog.pdf)

## Multiplayer

Both crew members need V4.2.0, including the matching Saved Games scripts (`Scripts/DCMII_MC_V3` and `Scripts/Hooks/DCMII_MC_Role.lua`), and a server that supports the mod. Some servers reject modified DCS-root files through integrity checks; dedicated servers can use the Server Edition.

**Confirmed server:** Pixel Storm.

In multicrew, pilot and WSO must each request and complete rearm and refuel on their own client.

The leg kneeboard uses the DCS ownship export. On servers that do not allow it, the sheet may stay dark until the kneeboard is opened; the crew figures work normally.

## Known issues

- Incorrect pitch or horizontal stabilizer behavior may occur during multicrew flight-control handovers.
- Singleplayer: the HUD-repeater camera may still be visible through the front cockpit seat (fixed in multiplayer).

## Known limits

Intentionally not synchronized between the seats: the native SMS weapon counter, TGP/FCR cursor and target lock, the underlying native INS alignment, threat display and CMDS/ECM states, and IFF codes.

The night-vision, FLIR and Modern AMRAAM changes apply to all aircraft in DCS while the respective package is enabled.

## Community and support

- **Website:** [dcmii.de](https://dcmii.de)
- **Discord:** [discord.gg/d6KDEzaxX](https://discord.gg/d6KDEzaxX) — downloads, support tickets, release announcements
- **YouTube:** [@viper-spike](https://www.youtube.com/@viper-spike)

For support, open a ticket on Discord and include your DCS version, aircraft variant, a description of the problem and your `dcs.log` if possible.

## Credits

- **IDF Mods Project** — the original F-16I Sufa / F-16D mod and its aircraft variants
- **Kaiqi / Pobit** — Center Pedestal Display (CPD) and F16V Core (GBU-39/53)
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
