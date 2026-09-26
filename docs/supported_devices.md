# Supported devices

Support new devices: [contribute/porting.md](/docs/contribute/porting.md)  

### Quick-picks
- **modules:** AVATTO, Aubess, iHseno
- **switches:** Moes 1-3gang (any design, except Star Feather)

### Careful with
- generic 1-gang modules - might not support OTA conversion
- BSEED switches - too many variants (can't know which you'll receive)

### Legend

| Symbol | Meaning  |                    |                     |                |                |           |          |
| :----: | -------- | ------------------ | ------------------- | -------------- | -------------- | --------- | -------- |
|   🚧️   | Status   | 🟩️ Fully supported | 🟨️ Mostly supported | 🟧️ In progress | 🟥️ Unsupported |           |          |
|   📦️   | Build    | ✔️ Available       | ❌️ Unavailable      |                |                |           |          |
|   💡️   | Category | 🇲️ Module          | 🇸️ Switch           | 🇴️ Outlet      | 🇵 Plug        | 🇷️ Remote | 🇧️ Board | 
|   ⚡️   | Power    | 🔌️ Mains           | 🔋️ Battery          | 🔱️ USB         |                |           |          |
|   📲️   | Install  | 🛜️ Wireless        | ➿️ By wire          | ❓️ Unknown     |                |           |          |
|   🏭️   | MCU      | `TL` Telink        | `SL` Silicon Labs   | `NXP` NXP      |                |           |          |
|   🅰   | Variant  | 🅰                  | 🅱                  | 🅲             | 🅳              | 🅴        | 🅵        |

<!-------------------------------------------------------------------
  `supported.md` is generated. 
  
  Do not edit it directly! Instead, edit:
  - `device_db.yaml`             - add or edit devices
  - `supported_devices.md.jinja` - update the template
  - `make_supported_devices.py`  - update generation script

  Generate with: `make tools/update_supported_devices`
-------------------------------------------------------------------->

> [!IMPORTANT]  
> Identify your device by **Zigbee Manufacturer** and linked threads/stores!  
> *Z2M pages are sometimes generic.*

### Device list

| 🚧 | 📦 | 💡 | ⚡️ | 📲 |  🏭  | Zb&nbsp;Manufacturer <br> Zb&nbsp;Model | Name <br> Z2M&nbsp;page&nbsp;🔗 | Store | Threads | Status |
| -- | -- | -- | -- | -- | :--: | :-------------------------------------- | :------------------------------ | ----: | ------: | :----- |
|  | ✔️ | 🇧 | 🔌 | 🛜 | **TL** | `_TZ3000_fa20yzve` <br> `TS0002` | [JWCOM 2-gang switch](https://www.zigbee2mqtt.io/devices/TS0002.html) | [`Store`](https://www.mercadolivre.com.br/interruptor-inteligente-tecla-fisica-2-botoes-zigbee-branco/up/MLBU3393955846) |   | JWCOM 2-gang, ZTU module. Pinout from factory config block at 0xF8000 | 
|  | ✔️ | 🇧 | 🔌 | 🛜 | **TL** | `_TZ3000_nuz46z91` <br> `TS0003` | [JWCOM 3-gang switch](https://www.zigbee2mqtt.io/devices/TS0003.html) |   |   | JWCOM 3-gang, ZTU module. Pinout from factory config block at 0xF8000 | 
|  | ✔️ | 🇧 | 🔌 | ➿ | **TL** | `_TZ3210_ok0ggpk7` <br> `TS0003` | [Nova Digital NTZB-02 (2 switches + 1 socket)](https://www.zigbee2mqtt.io/devices/TS0003.html) |   |   | ZTU with 512KB flash. Socket channel has relay only, no button. C1 is shared network LED / key 2 indicator on stock FW. Pinout from multimeter (no factory config block). | 

Data from [`device_db.yaml`](/device_db.yaml)
