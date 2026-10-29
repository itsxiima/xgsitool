# XGSI Tool

**XGSI Tool** is a lightweight, automated tool designed to build OEM-based Generic System Images (GSI) from stock manufacturer firmware. It unpacks, modifies, and repackages firmware into flashable GSI builds compatible with Treble-supported Android devices.

---

## Supported OEM Systems

XGSI Tool can process images and firmware dumps from a wide variety of Android-based OEM skins, including:

- **Samsung** (One UI)
- **OPPO / OnePlus / Realme** (ColorOS / OxygenOS / Realme UI)
- **vivo / iQOO** (OriginOS / Funtouch OS)
- **Xiaomi** (HyperOS / MIUI)
- *And any other oem firmware*

---

## Prerequisites

Before running the tool, ensure you have the following packages installed:

- **Python 3.8+**
- Core command-line utilities: `git`, `wget`, `curl`, `tar`, `unzip`, `simg2img`, `e2fsprogs`

Clone the repository and install requirements:

```bash
git clone [https://github.com/itsxiima/xgsitool.git](https://github.com/itsxiima/xgsitool.git)
cd xgsi-tool
pip3 install -r requirements.txt
```

## Usage

```bash
python3 xgsi.py --gsi <path to firmware>
```

The tool will automatically recognize the firmware and make required patches!

*Tip: You can convert the system to 64_32 if necessary:*

```bash
python3 xgsi.py --gsi <path> --abi32
```

See the full list of features by using:

```bash
python3 xgsi.py --help
```
