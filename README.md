# ACC-Setting-Presets

Configuration presets for **Assetto Corsa Competizione**.

## 📁 Repository Structure

### Controls/
Controller mapping configurations.
- `PS5.json` - PlayStation 5 controller bindings

### Presets/

#### assistsJson/
Driver assist presets (1-4), controlling:
- Automatic gears, clutch, and engine switching
- Stability control levels
- Auto pit limiter/procedure/request
- Auto wipers and lights
- Ideal racing line display

#### carSetupJson/
Car-specific setups organized by vehicle and track. Includes **54 cars** across multiple classes:

| Class | Cars |
|-------|------|
| **GT3** | Audi R8 LMS / Evo / Evo II, AMR V8/V12 Vantage, Bentley Continental (2016/2018), BMW M4/M6, Ferrari 296/488/488 Evo, Ford Mustang, Honda NSX / Evo, Jaguar G3, Lamborghini Huracán / Evo / Evo2, Lexus RC F, McLaren 650S/720S/720S Evo, Mercedes AMG / Evo, Nissan GT-R (2017/2018), Porsche 991 GT3 R / 991II GT3 R / 992 GT3 R |
| **GT4** | Alpine A110, AMR V8 Vantage, Audi R8, BMW M4, Chevrolet Camaro GT4.R, Ginetta G55, KTM X-Bow, Maserati MC, McLaren 570S, Mercedes AMG, Porsche 718 Cayman |
| **GT2** | Audi R8 LMS GT2, KTM X-Bow GT2, Maserati MC20 GT2, Mercedes AMG GT2 |
| **Cup** | Ferrari 488 Challenge Evo, Lamborghini Huracán ST / ST Evo2, Porsche 991II/992 GT3 Cup |
| **Other** | BMW M2 CS Racing, Lamborghini Gallardo REX, Porsche 935, Porsche 991 GT2 RS MR |

#### realismJson/
Realism presets (1-4) for simulation authenticity settings.

#### trackStatusJson/
Track condition presets (0-6) for grip levels and surface states.

#### weatherJson/
Weather configuration files:
- `data[0-6].json` - Weather condition data
- `status[0-6].json` - Weather status settings

### VideoSettings/
Graphics configuration profiles:
- `RACE.json` - Optimized for racing (performance-focused)
- `REPLAY.json` - Enhanced visuals for replay viewing
- `VR.json` - Virtual reality optimized settings

## 🎮 Installation

ACC stores user configuration files in your Documents folder. Copy the presets to their respective locations:

```
📁 Documents\Assetto Corsa Competizione\
│
├── 📁 Config\
│   ├── controls.json          ← Copy from Controls/
│   └── menuSettings.json      ← Copy video settings here
│
├── 📁 Customs\
│   ├── 📁 assistsJson\        ← Copy from Presets/assistsJson/
│   ├── 📁 realismJson\        ← Copy from Presets/realismJson/
│   ├── 📁 trackStatusJson\    ← Copy from Presets/trackStatusJson/
│   └── 📁 weatherJson\        ← Copy from Presets/weatherJson/
│
└── 📁 Setups\
    └── 📁 [car_name]\         ← Copy from Presets/carSetupJson/
        └── 📁 [track_name]\
            └── setup.json
```

### Step-by-Step Instructions

#### Controls
1. Copy `Controls/PS5.json` to:
   ```
   Documents\Assetto Corsa Competizione\Config\
   ```
2. Rename to `controls.json` (backup your existing file first)

#### Car Setups
1. Copy the car folder(s) from `Presets/carSetupJson/` to:
   ```
   Documents\Assetto Corsa Competizione\Setups\
   ```
2. Setups will appear in-game under the car's setup menu for each track

#### Assists, Realism, Track Status & Weather
1. Copy the entire folders from `Presets/` to:
   ```
   Documents\Assetto Corsa Competizione\Customs\
   ```
2. If the `Customs` folder doesn't exist, create it
3. Select presets in-game from Settings → Assists / Realism menus

#### Video Settings
1. Open the desired `.json` file (RACE, REPLAY, or VR)
2. Copy the contents into your existing:
   ```
   Documents\Assetto Corsa Competizione\Config\menuSettings.json
   ```
3. Or replace the graphics-related values in your config

> **Note:** Always backup your existing configuration files before overwriting them!

## 📝 License

See [LICENSE](LICENSE) for details.
