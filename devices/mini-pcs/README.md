# Mini PCs

Compact, complete computers. Single-board computers stay in [their own section](../single-board-computers/README.md); TV sticks and thin clients are out of scope unless repurposed as computers.

## Mainstream map

Families are navigation hints, not compatibility claims. Always record the exact model, CPU, board revision, and network chipsets.

### Mini-PC specialists

| Vendor | Common families | Typical range |
|---|---|---|
| [Beelink](beelink.md) | EQ/EQi, SE/SER, GT/GTi/GTR, Mini S | Entry to workstation |
| [MINISFORUM](https://www.minisforum.com/?lang=en) | UM, NAB/NPB, AI X, AtomMan, MS | Entry to workstation/gaming |
| [GEEKOM](https://www.geekompc.com/mini-pc/) | Air, IT, GT, A, AX | Entry to performance |
| [GMKtec](https://www.gmktec.com/collections/mini-pc) | NucBox G/M/K, EVO | Entry to AI workstation |
| [ACEMAGIC](https://acemagic.com/collections/minipcs) | Vista, Kron, Tank, Retro | Entry to gaming |
| [CHUWI](https://www.chuwi.com/) | LarkBox, HeroBox, CoreBox, AuBox | Entry to performance |
| [AOOSTAR](https://aoostar.com/collections/mini-pc) | GEM, GOD, MACO, G-FLIP | Performance, gaming, NAS hybrids |
| [BOSGAME](https://www.bosgame.com/) | E, P, M, VT series | Entry to AI workstation |
| [TRIGKEY](https://trigkey.com/en-gb) | G, Green, S, Speed | Entry to performance |

### Large OEMs and business micros

| Vendor | Common families | Why they matter |
|---|---|---|
| [Apple](https://www.apple.com/mac-mini/) | Mac mini | Apple silicon and macOS |
| [ASUS](https://www.asus.com/displays-desktops/nucs/nuc-mini-pcs/filter?Series=All-Series) | NUC Pro/Essential/Performance, ROG NUC, ExpertCenter PN | Current NUC steward; consumer to gaming |
| [Lenovo](https://www.lenovo.com/us/en/c/desktops/thinkcentre/m-series-tiny/) | ThinkCentre Tiny, ThinkStation Tiny | Common business and refurbished systems |
| [HP](https://www.hp.com/us-en/shop/vwa/desktops/form%3DMini) | Pro Mini, Elite Mini, Z2 Mini | Business and workstation models |
| [Dell](https://www.dell.com/en-us/shop/desktop-computers/scr/desktops/appref=mf-micro) | Dell Pro Micro, OptiPlex Micro, Precision Compact | Business fleet and refurbished systems |
| [MSI](https://us-store.msi.com/cubi-series?limit=24) | Cubi, PRO DP | Business and home-office systems |
| [Acer](https://www.acer.com/us-en/desktops-and-all-in-ones/veriton-business-desktops/veriton-vero-mini) | Veriton Mini | 1-litre business systems |
| [Fujitsu](https://www.fujitsu.com/global/imagesgig5/RS76301_Fujitsu_Desktop_ESPRIMO_MiniPC_Brochure.pdf) | ESPRIMO G/Q | Regional business and refurbished systems |

### Barebones, fanless, and compact workstations

| Vendor | Common families | Typical distinction |
|---|---|---|
| [ASRock](https://www.asrock.com/nettop/) | DeskMini, 4X4 BOX, NUC BOX | Socketed/barebone and embedded options |
| [GIGABYTE](https://www.gigabyte.com/Mini-PcBarebone?lan=en) | BRIX, BRIX Extreme, BRIX Pro | Barebones and industrial variants |
| [ZOTAC](https://www.zotac.com/us/product/mini_pcs/all?l=en) | ZBOX M/C/P/Q, MAGNUS, ZBOX Pro | Fanless through discrete-GPU systems |
| [Shuttle](https://www.shuttle.eu/en/products) | XPC nano, slim, cube | Barebones with more expansion choices |
| [ECS](https://www.ecs.com.tw/en/Product/Mini-PC) | LIVA Q/Z/One | Palm-size and embedded systems |
| [Simply NUC](https://simplynuc.com/mini-pcs/) | Onyx, Moonstone, extremeEdge | NUC-style systems and deployments |

### Legacy worth tracking

- **Intel NUC:** [Intel transferred NUC 7–13 support to ASUS](https://www.intel.com/content/www/us/en/support/articles/000097279/intel-nuc.html); ASUS develops current NUC systems. Older Intel-branded units remain common.
- **Older business micros:** Dell OptiPlex Micro, HP EliteDesk/ProDesk Mini, Lenovo ThinkCentre Tiny, and Fujitsu ESPRIMO Q are widely available used. Generation and form factor matter more than the family name.

## Choose by use

| Use | Start with | Check first |
|---|---|---|
| Home server / automation | Business micro, Beelink EQ/SER, GEEKOM, GMKtec | Idle power, NIC, storage, Linux support |
| Desktop | Mac mini, ASUS NUC, business micro, specialist Ryzen/Intel models | Display outputs, noise, RAM |
| Router / firewall | Multi-LAN specialist or industrial model | NIC vendor, IOMMU, BIOS recovery |
| Media center | Entry mini PC or fanless ZBOX/LIVA | Codec decode, HDMI version, CEC |
| Gaming / GPU work | ROG NUC, AtomMan, ZBOX MAGNUS, GT/GTR | GPU power limit, thermals, PSU |
| Lab / virtualization | Business micro or workstation mini | RAM ceiling, dual NIC, storage slots |

## Before adding a model

- Use the full model/SKU—not the storefront title.
- Note barebone vs preconfigured; RAM, SSD, Wi-Fi, and OS may differ.
- Save the vendor support page and BIOS version before reinstalling.
- Treat Linux support, USB4/Thunderbolt, suspend, audio, and Wi-Fi as separate tests.
- Reinstall or verify a preloaded OS before trusting it with credentials.

Copy the [device template](../../templates/device.md) to `vendor-model.md`, then add verified relationships to [Compatibility](../../COMPATIBILITY.md).
