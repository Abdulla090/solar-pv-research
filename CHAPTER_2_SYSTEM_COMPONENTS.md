# CHAPTER 2: SYSTEM COMPONENTS AND WORKING PRINCIPLES

---

## 2.1 Overview

The design and implementation of residential photovoltaic (PV) systems — whether on-grid or hybrid — require an in-depth understanding of the individual components that constitute the system, their operating principles, and how they interact to form a cohesive energy generation and management architecture. This chapter presents a detailed examination of the core components used in residential solar PV systems: solar photovoltaic modules, inverters, battery energy storage systems, and grid connection mechanisms including net metering. Each component is discussed in terms of its physical principles, key performance parameters, available technology variants, and role within both on-grid and hybrid system configurations.


---

## 2.2 Solar Photovoltaic (PV) Modules

### 2.2.1 Operating Principle: The Photovoltaic Effect

Solar photovoltaic modules are the primary energy conversion elements in any solar energy system. They convert incident solar radiation directly into electrical energy through the photovoltaic effect — a quantum mechanical process first observed by Alexandre-Edmond Becquerel in 1839 and first practically demonstrated by Bell Laboratories in 1954 with a silicon-based solar cell achieving approximately 6% efficiency (Chapin et al., 1954).

The photovoltaic effect occurs within semiconductor materials — most commonly crystalline silicon (Si) — that are engineered to contain a p-n junction. When photons from sunlight strike the semiconductor surface with energy greater than or equal to the material's bandgap energy (approximately 1.12 eV for silicon), they transfer energy to valence electrons, exciting them into the conduction band and creating electron-hole pairs. The internal electric field at the p-n junction separates these charge carriers: electrons are swept toward the n-type (phosphorus-doped) layer, while holes migrate toward the p-type (boron-doped) layer. This charge separation establishes a potential difference (voltage) across the cell, and when an external circuit is connected, current flows — converting solar energy into usable direct current (DC) electricity (Green, 2003; Luque and Hegedus, 2011).

**[INSERT Figure 2.1: The conversion of solar radiation to electricity in PV systems, showing the p-n junction, photon absorption, electron flow, and hole flow mechanisms.]**

The key electrical parameters that characterize a PV cell's performance under Standard Test Conditions (STC: irradiance of 1000 W/m², cell temperature of 25°C, and air mass AM1.5) are:

- **Open-Circuit Voltage (Voc):** The maximum voltage produced by the cell when no current flows (open circuit). For a typical crystalline silicon cell, Voc ranges from 0.5 to 0.7 V.

- **Short-Circuit Current (Isc):** The maximum current produced when the cell terminals are short-circuited (zero voltage). Isc is directly proportional to the incident solar irradiance and the cell's active area.

- **Maximum Power Point (Pmax):** The operating point on the cell's current-voltage (I-V) characteristic curve where the product of voltage and current is maximized. This is the point at which the cell delivers maximum electrical power.

- **Maximum Power Voltage (Vmp) and Current (Imp):** The voltage and current values at the maximum power point, respectively.

- **Fill Factor (FF):** A dimensionless parameter representing the "squareness" of the I-V curve, defined as the ratio of Pmax to the product of Voc and Isc. Typical FF values for high-quality crystalline silicon cells range from 0.75 to 0.85.

- **Conversion Efficiency (eta):** The ratio of electrical power output to incident solar power, expressed as a percentage.

The relationship among these parameters is expressed by the fundamental PV equation:

    Pmax = Vmp x Imp = FF x Voc x Isc

    eta = Pmax / (G x A)

Where G is the solar irradiance (W/m²) and A is the cell area (m²).

### 2.2.2 PV Module Construction and Types

A PV module consists of multiple individual cells electrically connected in series and parallel configurations to achieve the desired output voltage and current ratings. Cells are encapsulated between a front glass cover and a rear backsheet (or glass-glass construction in bifacial modules), with ethylene vinyl acetate (EVA) encapsulant providing mechanical protection, moisture resistance, and optical coupling. An aluminum frame provides structural rigidity and mounting compatibility, while a junction box on the rear side provides electrical interconnection terminals.

The principal types of crystalline silicon PV modules used in residential applications are:

**Table 2.1: Comparison of Major PV Module Technologies**

| Parameter | Monocrystalline Si | Polycrystalline Si | Thin-Film (CdTe/CIGS) |
|---|---|---|---|
| Cell Efficiency | 18–24% | 16–20% | 10–13% |
| Module Efficiency | 17–22% | 15–18% | 9–12% |
| Temperature Coefficient | -0.3 to -0.4 %/°C | -0.4 to -0.5 %/°C | -0.2 to -0.3 %/°C |
| Degradation Rate | 0.3–0.5 %/year | 0.5–0.7 %/year | 0.5–1.0 %/year |
| Lifespan | 25–30+ years | 25–30 years | 20–25 years |
| Space Efficiency | High | Medium | Low |
| Cost per Watt | Moderate–High | Low–Moderate | Low |
| Appearance | Uniform dark (black/navy) | Blue multi-toned | Uniform thin profile |
| Best Application | Space-constrained rooftops | Budget-conscious installations | Large-area, low-weight applications |

Monocrystalline silicon modules currently dominate the residential market due to their superior efficiency, better aesthetic appearance, favorable temperature coefficients, and declining price premiums. The transition from older PERC (Passivated Emitter and Rear Cell) manufacturing to advanced cell architectures — TOPCon (Tunnel Oxide Passivated Contact) and HJT (Heterojunction Technology) — has further improved monocrystalline module efficiencies while reducing light-induced degradation (LID) and potential-induced degradation (PID) (LONGi, 2024; Green et al., 2022).

### 2.2.3 Environmental Factors Affecting PV Module Performance

PV module output is influenced by several environmental parameters beyond irradiance:

- **Temperature:** Module efficiency decreases with increasing cell temperature. The temperature coefficient (typically -0.3 to -0.5 %/°C for crystalline silicon) quantifies this effect. In Erbil, where summer ambient temperatures routinely exceed 43°C and rooftop module temperatures can reach 60–70°C, temperature-induced losses can reduce output by 15–20% relative to STC ratings (Skoplaki and Palyvos, 2009).

- **Soiling and Dust:** Accumulation of dust, sand, and particulate matter on the module surface reduces optical transmittance and, consequently, power output. Studies in arid Middle Eastern climates have reported soiling losses of 15–30% without regular cleaning (Mani and Pillai, 2010). In the Kurdistan Region, where dry, dusty conditions prevail during summer months, periodic cleaning is essential for maintaining system performance.

- **Wind Speed:** Wind has a dual effect on PV systems. Moderate wind speeds improve module performance by providing convective cooling, reducing cell temperature, and partially mitigating temperature-induced efficiency losses. However, extreme wind speeds can cause structural damage to mounting systems if not properly designed for local wind load conditions.

- **Shading:** Even partial shading of a PV module can disproportionately reduce system output due to the series-connected nature of cells within a string. When one cell is shaded, it acts as a resistance rather than a power source, potentially causing "hot spots" and triggering bypass diode activation, which reduces the output of the entire string. Proper site assessment and shade analysis are therefore critical during system design.


---

## 2.3 Inverters

### 2.3.1 Function and Operating Principle

Inverters are essential power electronics components that perform the conversion of direct current (DC) electricity generated by PV modules into alternating current (AC) electricity compatible with residential electrical systems and the utility grid. In addition to DC-to-AC conversion, modern inverters perform several critical functions:

- **Maximum Power Point Tracking (MPPT):** Continuously adjusting the operating voltage and current of the PV array to extract maximum power under varying irradiance and temperature conditions. MPPT algorithms (such as Perturb and Observe, Incremental Conductance, or advanced machine-learning-based algorithms) typically achieve tracking efficiencies exceeding 99% (Esram and Chapman, 2007).

- **Grid Synchronization:** In grid-connected systems, the inverter must synchronize its output frequency (50 Hz in Iraq), voltage, and phase with the utility grid to ensure safe and stable power injection.

- **Anti-Islanding Protection:** Grid-tied inverters incorporate safety mechanisms that automatically disconnect the PV system from the grid during utility outages, preventing dangerous back-feeding of power to the grid that could endanger utility workers (IEEE Standard 1547, 2018).

- **System Monitoring and Data Logging:** Modern inverters incorporate communication interfaces (Wi-Fi, Ethernet, RS485) that enable real-time monitoring of system performance parameters including power output, energy yield, voltage, current, frequency, and fault conditions.

- **Power Quality Management:** High-quality inverters minimize harmonic distortion in the AC output (typically maintaining Total Harmonic Distortion below 3–5%) and incorporate reactive power compensation capabilities.

### 2.3.2 Types of Inverters for Residential Applications

Three primary inverter topologies are used in residential PV systems:

**a) String Inverters:**
The most common and cost-effective solution for residential systems. A single centralized inverter receives the combined DC output from a series-connected "string" of PV modules and converts it to AC. String inverters are simple, reliable, and efficient (peak efficiencies of 96–98%), but their performance is limited by the weakest module in the string due to the series connection — making them susceptible to partial shading losses (Kjaer et al., 2005).

**b) Microinverters:**
Individual inverter units mounted directly on each PV module, performing module-level DC-to-AC conversion. Microinverters eliminate string-level mismatch losses, improve performance under partial shading conditions, and enable module-level monitoring. However, they incur higher per-watt costs and introduce more potential points of failure across the system (Enphase, 2024).

**c) Hybrid Inverters (Inverter-Chargers):**
Specialized inverters designed for hybrid PV-battery systems that integrate multiple functions: DC-to-AC conversion from the PV array, bidirectional battery charging and discharging, grid synchronization, and automatic transfer switching between grid-connected and islanded (off-grid) operating modes. Hybrid inverters incorporate sophisticated energy management algorithms that prioritize power flow according to programmed strategies — typically: (1) supply household load from solar, (2) charge batteries with excess solar, (3) export remaining surplus to grid, and (4) discharge batteries during peak demand or grid outages (Lai and Ellis, 2017).

For this study, a hybrid inverter configuration is employed for the hybrid system, while a standard string inverter is utilized for the on-grid system, enabling a direct comparison of the two approaches under identical PV array conditions.

**Table 2.2: Comparison of Inverter Types for Residential PV Systems**

| Parameter | String Inverter | Microinverter | Hybrid Inverter |
|---|---|---|---|
| Topology | Centralized | Distributed (per-module) | Centralized + battery interface |
| Peak Efficiency | 96–98% | 95–97% | 93–97% |
| MPPT | System-level (1–2 trackers) | Module-level | System-level + battery MPPT |
| Shading Tolerance | Low | High | Low–Medium |
| Battery Integration | No (external required) | No | Yes (built-in) |
| Islanding Capability | No (anti-islanding) | No | Yes (automatic transfer) |
| Cost (per Watt) | Lowest | Highest | Moderate–High |
| Monitoring Granularity | System-level | Module-level | System + battery level |
| Typical Lifespan | 10–15 years | 15–25 years | 10–15 years |
| Best Application | Standard on-grid systems | Shading-prone rooftops | Hybrid PV-battery systems |


---

## 2.4 Battery Energy Storage Systems (BESS)

### 2.4.1 Role of Battery Storage in Residential PV Systems

Battery energy storage systems address the fundamental temporal mismatch between solar energy generation (predominantly during daytime hours) and residential electricity consumption (which typically peaks during evening hours). In hybrid PV systems, batteries serve several critical functions:

- **Energy Time-Shifting:** Storing excess solar energy generated during peak irradiance periods for consumption during evening or nighttime hours, thereby increasing the solar self-consumption ratio from a typical 30–40% (without storage) to 60–80% (with appropriately sized storage) (Koskela et al., 2019).

- **Backup Power:** Providing continuous electricity supply during grid outages — a critically important function in the Kurdistan Region, where grid interruptions, though improving, remain a recurring concern.

- **Peak Shaving:** Reducing grid imports during high-demand (and potentially high-tariff) periods by discharging stored energy, thereby lowering electricity costs under time-of-use tariff structures.

- **Grid Support:** In advanced implementations, batteries can provide grid support services including frequency regulation and voltage stabilization, though this functionality is not yet widely deployed in the Iraqi residential context.

### 2.4.2 Battery Technologies for Residential Applications

The two principal battery technologies deployed in residential solar systems are:

**a) Lead-Acid Batteries:**
The oldest and most established rechargeable battery technology, available in flooded (FLA) and valve-regulated (VRLA) variants including absorbed glass mat (AGM) and gel types. Lead-acid batteries offer low upfront costs but are characterized by limited cycle life (300–1,500 cycles), moderate depth of discharge (DoD) limits (typically 50% for longevity), heavy weight, and higher maintenance requirements. Their round-trip efficiency is approximately 75–85%.

**b) Lithium-Ion Batteries:**
The dominant technology for modern residential energy storage, utilizing various cathode chemistries including lithium iron phosphate (LiFePO4/LFP), lithium nickel manganese cobalt oxide (NMC), and lithium nickel cobalt aluminum oxide (NCA). Lithium-ion batteries offer substantially superior performance across virtually all metrics: higher energy density (150–250 Wh/kg vs. 30–50 Wh/kg for lead-acid), deeper permissible discharge (80–100% DoD), longer cycle life (3,000–10,000+ cycles for LFP), higher round-trip efficiency (90–98%), lighter weight, and lower maintenance requirements. LFP chemistry is increasingly preferred for residential applications due to its excellent thermal stability, non-toxicity, and extended cycle life, despite slightly lower energy density compared to NMC (Zakeri and Syri, 2015; Hesse et al., 2017).

**Table 2.3: Comparison of Battery Technologies for Residential PV Systems**

| Parameter | Lead-Acid (VRLA) | Lithium-Ion (NMC) | Lithium Iron Phosphate (LFP) |
|---|---|---|---|
| Energy Density | 30–50 Wh/kg | 150–220 Wh/kg | 90–160 Wh/kg |
| Cycle Life (at 80% DoD) | 300–800 cycles | 2,000–4,000 cycles | 3,000–10,000 cycles |
| Recommended DoD | 50% | 80–90% | 80–100% |
| Round-Trip Efficiency | 75–85% | 90–95% | 92–98% |
| Self-Discharge Rate | 3–5% per month | 1–3% per month | 1–2% per month |
| Operating Temperature | -20 to 50°C | -10 to 45°C | -20 to 60°C |
| Calendar Life | 3–5 years | 8–12 years | 10–15 years |
| Maintenance | Moderate (FLA) / Low (VRLA) | Low | Very Low |
| Safety | Hydrogen off-gassing risk | Thermal runaway risk | Excellent thermal stability |
| Cost per kWh (2024) | $100–$200 | $250–$400 | $200–$350 |
| Best Application | Budget systems, backup only | High energy density needs | Long-life residential storage |

### 2.4.3 Battery Sizing Considerations

Proper battery sizing is critical to achieving the desired balance between system cost, energy autonomy, and component longevity. The required battery capacity (Cbatt) can be estimated using the following relationship:

    Cbatt (Wh) = (Enight x Dautonomy) / (DoD x eta_batt)

Where:
- Enight = daily energy consumption during non-solar hours (Wh)
- Dautonomy = desired number of days of autonomous operation (typically 1–2 days for hybrid systems)
- DoD = maximum depth of discharge (0.8 for LFP, 0.5 for lead-acid)
- eta_batt = battery round-trip efficiency (0.90–0.95 for lithium-ion)

Over-sizing the battery increases capital costs without proportional benefit, while under-sizing reduces backup capability and accelerates degradation through deep cycling. Research by Khezri et al. (2020) and Hesse et al. (2017) has demonstrated that optimal battery sizing requires detailed analysis of the specific household load profile rather than generic rule-of-thumb approaches.


---

## 2.5 Grid Connection and Net Metering

### 2.5.1 Grid Interconnection

Grid interconnection enables bidirectional power flow between the residential PV system and the utility network. In an on-grid configuration, the PV system operates as a supplementary power source to the grid: when solar generation exceeds household demand, excess electricity is exported to the grid; when generation is insufficient, electricity is imported from the grid. This bidirectional power exchange is managed by the grid-tied inverter, which ensures that all exported power meets grid code requirements for voltage, frequency, power quality, and safety.

Grid interconnection requires compliance with applicable interconnection standards, which in most jurisdictions are based on IEEE Standard 1547 (Standard for Interconnection and Interoperability of Distributed Energy Resources) and IEC 61727 (Photovoltaic Systems — Characteristics of the Utility Interface). These standards specify requirements for:

- Voltage and frequency operating ranges
- Power quality (harmonic distortion limits)
- Anti-islanding detection and response time
- Reconnection procedures following grid restoration
- Grounding and protection coordination

### 2.5.2 Net Metering

Net metering is an electricity billing mechanism that credits PV system owners for the surplus electricity they export to the grid. Under a net metering arrangement, a bidirectional electricity meter records both imported and exported energy, and the consumer is billed for the net difference. When the PV system generates more electricity than consumed in a billing period, the excess credit is typically carried forward to subsequent billing cycles.

The economic impact of net metering depends critically on the credit rate applied to exported electricity. In a "one-to-one" net metering scheme, exported electricity is credited at the full retail rate, maximizing economic benefit to the PV system owner. In other arrangements, such as "net billing" or "buy-all-sell-all" schemes, the export rate may be lower than the retail rate, reducing the economic incentive for grid-connected operation.

In the Iraqi context, net metering policies are still in the early stages of development. The Kurdistan Regional Government has begun implementing regulatory frameworks to support distributed solar generation, but the absence of mature net metering regulations currently limits the economic optimization of purely on-grid systems in the region — further strengthening the case for hybrid systems with self-consumption optimization capabilities.


---

## 2.6 System Architectures: On-Grid vs. Hybrid

### 2.6.1 On-Grid System Architecture

An on-grid (grid-tied) residential PV system consists of three primary components: the PV array, a grid-tied inverter, and the electrical balance-of-system (BOS) components including wiring, protection devices, and metering. The system architecture is straightforward:

    PV Array --> DC Wiring --> Grid-Tied Inverter --> AC Distribution Panel --> Household Loads / Grid

**[INSERT Figure 2.2: Schematic diagram of a typical on-grid residential PV system showing power flow from PV array through inverter to household loads and grid connection.]**

Key characteristics of on-grid systems:
- No battery storage — all surplus energy is exported to the grid
- System ceases operation during grid outages (anti-islanding)
- Lowest capital cost and system complexity
- Performance dependent on grid availability and net metering policies
- Highest conversion efficiency (no battery charge/discharge losses)

### 2.6.2 Hybrid System Architecture

A hybrid residential PV system adds battery energy storage and a hybrid inverter (or separate charge controller) to the on-grid architecture, creating a more versatile energy management platform:

    PV Array --> DC Wiring --> Hybrid Inverter <--> Battery Bank
                                    |
                                    v
                            AC Distribution Panel --> Household Loads / Grid

**[INSERT Figure 2.3: Schematic diagram of a hybrid residential PV system showing bidirectional power flow between PV array, battery storage, household loads, and grid connection.]**

The hybrid inverter manages power flow according to a priority-based algorithm:
1. **Priority 1:** Supply household loads directly from solar generation
2. **Priority 2:** Charge batteries with excess solar energy
3. **Priority 3:** Export remaining surplus to grid (if net metering available)
4. **Priority 4:** During low solar / nighttime, discharge batteries to supply loads
5. **Priority 5:** Import from grid only when both solar and battery are insufficient

During grid outages, the hybrid inverter automatically isolates from the grid (islanding mode) and continues supplying critical loads from battery storage and/or solar generation, providing uninterrupted power supply — a decisive advantage in regions with unreliable grid infrastructure.

**Table 2.4: Comparative Summary of On-Grid vs. Hybrid System Architectures**

| Feature | On-Grid System | Hybrid System |
|---|---|---|
| Core Components | PV array + grid-tied inverter | PV array + hybrid inverter + battery |
| Battery Storage | None | Yes (lithium-ion or lead-acid) |
| Grid Dependency | High (no power during outages) | Medium (battery backup available) |
| Self-Consumption Rate | 30–40% (typical) | 60–80% (with optimized storage) |
| Capital Cost | Lower | Higher (30–60% premium for battery) |
| System Complexity | Low | Medium–High |
| Maintenance | Minimal | Moderate (battery monitoring) |
| Energy Independence | Low | Medium–High |
| Anti-Islanding | Yes (shuts down during outage) | Bypass (operates in island mode) |
| Conversion Efficiency | Higher (no battery losses) | Slightly lower (battery round-trip losses of 5–10%) |
| Optimal Context | Stable grid, favorable net metering | Unstable grid, high self-consumption goals |
| Suitability for Erbil | Limited (grid instability concerns) | Highly suitable |


---

## 2.7 Chapter Summary

This chapter has presented a detailed examination of the core components and working principles underlying residential photovoltaic systems. The discussion covered:

1. **PV modules** — their operating principle based on the photovoltaic effect in semiconductor p-n junctions, key electrical parameters (Voc, Isc, Pmax, FF, efficiency), module construction, available technologies (monocrystalline, polycrystalline, thin-film), and the environmental factors (temperature, soiling, wind, shading) that influence performance under real operating conditions in Erbil's hot, arid climate.

2. **Inverters** — their essential role in DC-to-AC conversion, MPPT optimization, grid synchronization, and system protection, with a comparative evaluation of string inverters, microinverters, and hybrid inverters appropriate for the on-grid and hybrid configurations investigated in this study.

3. **Battery energy storage systems** — their function in addressing the temporal mismatch between solar generation and residential consumption, a comparative analysis of lead-acid versus lithium-ion (LFP) technologies, and the principles governing optimal battery capacity sizing for residential hybrid systems.

4. **Grid connection and net metering** — the technical requirements for grid interconnection, the economic mechanisms of net metering, and the current status of these policies in the Iraqi and Kurdistan Region context.

5. **System architectures** — a systematic comparison of on-grid and hybrid configurations, their power flow management strategies, and their respective advantages and limitations in the context of Erbil's energy landscape.

The theoretical foundations and component specifications established in this chapter provide the basis for the system design calculations, experimental methodology, and performance analysis presented in the subsequent chapters.
