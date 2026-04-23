# CHAPTER 1: INTRODUCTION

## 1.1 Background

The escalating global demand for electricity, driven by rapid population growth, urbanization, and industrial expansion, has placed unprecedented pressure on conventional power generation infrastructure worldwide. According to the International Energy Agency (IEA, 2024), global electricity consumption surpassed 29,000 TWh in 2024, with projections indicating a continued annual growth rate of 3.4% through 2030. This rising demand, coupled with the urgent need to mitigate climate change and reduce greenhouse gas (GHG) emissions, has catalyzed a paradigm shift toward renewable energy sources, with solar photovoltaic (PV) technology emerging as one of the most scalable, cost-effective, and rapidly deployable solutions available (IRENA, 2024).

The global solar PV market has witnessed extraordinary expansion in recent years. Cumulative installed PV capacity exceeded 2.2 terawatts (TW) by the end of 2024 and reached approximately 2.8 TW by mid-2025, with annual capacity additions surpassing 600 GW (IEA-PVPS, 2025; REN21, 2025). Solar PV alone accounted for approximately 7% of global electricity generation in 2024, increasing to 8.8% in the first half of 2025, and for the first time in history, a modern renewable energy source led absolute global energy demand expansion (Ember Energy, 2025; PV Tech, 2025). This remarkable trajectory has been fueled by an unprecedented decline in technology costs: the price per watt of PV modules has fallen by approximately 85-90% since 2010, while the installed cost of residential systems has decreased from $8.00-$9.00/W to approximately $2.50-$3.50/W over the same period (Our World in Data, 2024; NREL, 2024). The global benchmark levelized cost of electricity (LCOE) for utility-scale solar reached $0.039/kWh in 2025 (BNEF, 2025), making solar energy cheaper than fossil-fuel-generated electricity in the majority of global markets.

Within this global context, distributed residential PV systems have emerged as a particularly significant segment. Distributed solar installations added nearly 200-220 GW globally in 2024 alone (REN21, 2025). Residential PV systems enable electricity generation at the point of consumption, reducing transmission losses, enhancing energy security, and empowering households with greater control over their energy costs and carbon footprint. The proliferation of residential solar has been accelerated by supportive policy mechanisms such as net metering, feed-in tariffs, tax incentives, and declining battery storage costs (Rai and Robinson, 2013; Parida et al., 2011).

The Republic of Iraq, with a population of approximately 46.1 million as of 2025 (Iraq Census, 2025), faces one of the most severe and persistent electricity crises in the MENA region. Iraq's energy sector is almost entirely dependent on fossil fuels, with oil and natural gas accounting for approximately 99% of electricity generation (EIA, 2024). The country's CO2 emissions reached approximately 233 million tonnes in 2023, rising to 239 million tonnes in 2024, with a per capita emission rate of approximately 5.19 tonnes (Worldometers, 2024). Despite government plans to increase power generation capacity to 44 GW, Iraq continues to face a persistent supply-demand gap estimated at approximately 10,000 MW, with technical and commercial losses accounting for 50-60% of generated electricity (Rudaw Research Center, 2024). The residential sector is the largest consumer of electricity in Iraq, accounting for approximately 65% of total national consumption (IEA, 2024), driven primarily by space cooling demands during extreme summer temperatures exceeding 43 degrees Celsius.

The Kurdistan Region of Iraq (KRI), and its capital Erbil in particular, presents a unique case study for residential solar energy deployment. Located at approximately 36.19 N latitude and 44.01 E longitude, at an elevation of approximately 420 meters above sea level, Erbil experiences a hot semi-arid climate. The city receives an annual average of approximately 9 hours of sunshine per day, with summer sunshine exceeding 12-14 hours daily. The annual global horizontal irradiation (GHI) in the Kurdistan Region ranges between 1,800 and 2,390 kWh/m2/year, with daily GHI values of 4.4-5.6 kWh/m2/day (Global Solar Atlas, 2024), representing exceptionally favorable conditions for photovoltaic energy harvesting. The Kurdistan Regional Government (KRG) has set an ambitious target of achieving 3 GW of solar power capacity by 2033 and launched the "Runaki" (Light) project in late 2024 (KRG Ministry of Electricity, 2024).

Historically, Iraqi households have been heavily reliant on private diesel generators. Households subscribe to neighborhood-based generator services at costs of 10,000-30,000 Iraqi Dinars per ampere per month, with total monthly expenditures reaching 40,000-200,000 IQD ($30-$150 USD) depending on seasonal demand (Rudaw, 2024; IntechOpen, 2023). These diesel generators constitute a significant source of air pollution (CO2, CO, NOx, SOx, and particulate matter), noise pollution, and soil contamination. The transition from diesel generator dependency to residential solar PV systems therefore represents both an economic imperative and an environmental and public health necessity.

Two primary configurations of residential solar PV systems are commonly deployed: on-grid (grid-tied) systems and hybrid systems. On-grid systems operate in direct connection with the utility network, allowing households to consume generated solar electricity while relying on the grid during periods of insufficient production (Lund and Kempton, 2008). These systems are characterized by lower capital costs but automatically shut down during grid outages (Enphase, 2024). In contrast, hybrid PV systems integrate battery energy storage systems (BESS) with grid connectivity, enabling households to store excess solar generation, implement peak-shaving strategies, and maintain power supply during grid interruptions (Zakeri and Syri, 2015). While hybrid systems incur higher capital costs, they offer substantially greater energy autonomy and supply reliability (Lund et al., 2025).

Given the unique intersection of abundant solar resources, chronic electricity deficits, heavy reliance on polluting diesel generators, and an evolving regulatory landscape in the Kurdistan Region, this research undertakes a comprehensive comparative analysis of hybrid and on-grid solar PV systems for residential applications in Erbil.


## 1.2 Literature Review

### 1.2.1 Evolution of Solar PV Technology and Cost Trends

The photovoltaic effect was first observed by Alexandre-Edmond Becquerel in 1839. Modern PV cells are predominantly manufactured from crystalline silicon (Green et al., 2022). Commercially available monocrystalline silicon cells achieve efficiencies of 18-24%, while polycrystalline cells typically achieve 16-20% (Parida et al., 2011; NREL, 2024).

The transition from PERC technology to next-generation architectures — TOPCon, HJT, and IBC — has pushed commercial efficiencies to new heights (LONGi, 2024). Perovskite-on-silicon tandem solar cells have achieved certified laboratory efficiencies exceeding 34%, surpassing the Shockley-Queisser limit for single-junction silicon cells (LONGi, 2024; PV Magazine, 2024). Modern PV modules exhibit median degradation rates of approximately 0.5-0.6% per year, ensuring systems retain approximately 87-90% of original output after 25 years (NREL, 2023; Jordan and Kurtz, 2013).

### 1.2.2 Residential On-Grid PV Systems

On-grid systems have been widely studied for residential applications due to their simplicity and lower upfront costs. Rawat et al. (2024) demonstrated that on-grid systems effectively meet household demand at significantly lower installation costs than hybrid alternatives. Hassan (2021) found that on-grid systems offer lower life-cycle costs in urban settings with reliable grid availability.

However, anti-islanding protection causes on-grid systems to disconnect during outages. This limitation has been identified as a critical barrier in developing countries with unreliable electricity infrastructure (Walker, 2013; Zelazna et al., 2020).

### 1.2.3 Hybrid PV Systems with Battery Energy Storage

Hybrid PV-battery systems enable excess solar generation to be stored and dispatched during evening peak demand or grid outages (Zakeri and Syri, 2015). Shah et al. (2015) found that hybrid configurations significantly reduce energy bills and carbon footprints. Zelazna et al. (2020) concluded that hybrid PV systems are highly competitive when environmental and technological factors are weighted alongside economic considerations. Serat et al. (2024) identified polycrystalline hybrid PV systems paired with battery storage as the most cost-effective configuration for energy autonomy.

Battery sizing and optimization are critical determinants of hybrid system performance. Hesse et al. (2017) demonstrated that optimal battery sizing must account for specific household load profiles. Li et al. (2019) found that optimization can reduce grid imports by 60-80%. Koskela et al. (2019) showed that proper battery sizing can increase self-consumption by over 30%. Gabr et al. (2021) demonstrated that multi-objective optimization results in significantly shorter payback periods. Khezri et al. (2020) provided a universal methodology using Net Present Cost minimization. Shabbir et al. (2017) confirmed that detailed load-curve analysis is necessary for optimal battery sizing.

### 1.2.4 Solar Energy Potential and Electricity Context in Iraq

Despite receiving annual GHI values of 1,800-2,390 kWh/m2/year and approximately 2,979 hours of annual sunshine, renewable energy accounted for only 1-2% of Iraq's total electricity generation as of 2025 (IRENA, 2024; EIA, 2024). The federal government has set a target of 12 GW of renewable energy by 2030 and announced a $6 billion investment drive in late 2025 (Switchgear Magazine, 2025). GIS-based solar radiation mapping has demonstrated that solar radiation intensity increases from north to south across the Kurdistan Region (ResearchGate, 2023). However, existing Iraqi solar research has focused on theoretical assessment rather than practical field performance evaluation.

### 1.2.5 System Design Methodologies

Residential PV system design involves load assessment, system sizing, component selection, and installation optimization (Bandyopadhyay et al., 2020). System sizing calculations must account for average daily solar irradiation, module efficiency, temperature derating, system losses, and desired energy autonomy (Mulleriyawage et al., 2020). For hybrid systems, battery capacity determination requires consideration of daily energy consumption, backup duration, depth of discharge limits, and cycle life characteristics (Shabbir et al., 2017). Tilt angle and orientation optimization are essential, with the ideal tilt angle for Erbil approximating 30-35 degrees.


## 1.3 Research Gap

Despite the substantial body of literature, several critical gaps persist:

1. The majority of existing studies rely on simulated data rather than field-collected measurements under Erbil's specific conditions.

2. Most published studies employ generic household load profiles that do not reflect the unique consumption patterns of Iraqi households, characterized by extreme cooling loads and diesel generator dependence.

3. Few studies have conducted direct, side-by-side comparisons of on-grid and hybrid configurations under identical conditions within the Iraqi context.

4. Existing literature rarely quantifies the benefits of solar PV in terms of displacing private diesel generator usage — a unique feature of the Iraqi energy landscape.

5. The rapidly evolving regulatory landscape in the Kurdistan Region has not been adequately incorporated into existing system design frameworks.


## 1.4 Objectives of the Study

The primary aim is to develop a practical, locally grounded framework for the design, performance evaluation, and techno-economic comparison of hybrid and on-grid residential PV systems in Erbil. Specific objectives:

1. To collect and analyze field-measured experimental data on PV system parameters under real operating conditions in Erbil.

2. To design and size residential on-grid and hybrid PV systems based on measured performance data and actual household energy demand.

3. To evaluate and compare on-grid and hybrid system performance in terms of energy yield, efficiency, capacity factor, and reliability.

4. To conduct a comprehensive techno-economic analysis comparing capital costs, operational costs, payback periods, and LCOE for both configurations.

5. To provide evidence-based, implementable recommendations for optimal residential PV system deployment in the Kurdistan Region.


## 1.5 Novelty and Contribution

- Field-based experimental validation using data from an actual PV installation in Erbil.
- Dual-configuration comparative framework under identical environmental conditions.
- Context-specific analysis integrating local climatic data, consumption patterns, tariff structures, and diesel generator displacement economics.
- Primary experimental data contribution to a geographically underserved research domain.


## 1.6 Significance of the Study

- Residential consumers can make informed PV system selection decisions.
- Energy policymakers can design more effective incentive programs aligned with the 3 GW by 2033 target.
- System designers can reference locally validated design parameters and performance benchmarks.
- The academic community benefits from primary field data in an underrepresented climate zone and socio-economic context.


## References

1. Bandyopadhyay, S., et al. (2020). Techno-Economical Model Based Optimal Sizing of PV-Battery Systems for Microgrids. IEEE Transactions on Sustainable Energy, 11(3), pp. 1657-1668.
2. Bloomberg New Energy Finance (BNEF) (2025). Global LCOE Benchmark. London: BNEF.
3. Ember Energy (2025). Global Electricity Review 2025. https://ember-energy.org
4. Energy Information Administration (EIA) (2024). Iraq Country Analysis Brief. Washington, DC.
5. Enphase Energy (2024). Grid-Tied vs. Hybrid Solar Systems. https://enphase.com
6. Gabr, A.Z., et al. (2021). Multiobjective Optimization of PV-Battery System Sizing. IEEE Access, 9, pp. 23816-23830.
7. Global Solar Atlas (2024). Solar Resource Map - Iraq. World Bank Group / ESMAP.
8. Green, M.A., et al. (2022). Solar cell efficiency tables (Version 60). Progress in Photovoltaics, 30(7), pp. 699-727.
9. Hassan, Q. (2021). Evaluation and optimization of off-grid and on-grid photovoltaic power system. Renewable Energy, 164, pp. 1086-1101.
10. Hesse, H., et al. (2017). Economic Optimization of Component Sizing for Residential Battery Storage. Energies, 10(7), 835.
11. International Energy Agency (IEA) (2024). World Energy Outlook 2024. Paris: OECD/IEA.
12. IEA-PVPS (2025). Snapshot of Global PV Markets 2025. Report T1-44.
13. IRENA (2024). Renewable Power Generation Costs in 2023. Abu Dhabi: IRENA.
14. Jordan, D.C. and Kurtz, S.R. (2013). Photovoltaic Degradation Rates. Progress in Photovoltaics, 21(1), pp. 12-29.
15. Khezri, R., et al. (2020). Optimal Capacity of Solar PV and Battery Storage. IEEE Trans. Industry Applications, 56(5), pp. 5319-5327.
16. Koskela, J., et al. (2019). Using electrical energy storage in residential buildings. Applied Energy, 239, pp. 1175-1189.
17. Kusakana, K. (2019). Reliability of autonomous solar-wind microgrids. Journal of Energy Storage, 21, pp. 406-413.
18. Li, J., et al. (2019). Optimal sizing of grid-connected photovoltaic battery systems. Renewable Energy, 136, pp. 1027-1038.
19. LONGi Green Energy (2024). World Record Solar Cell Efficiency Achievements. https://longi.com
20. Lund, P.D. and Kempton, W. (2008). Integration of renewable energy into transport and electricity sectors. Energy Policy, 36(9), pp. 3578-3587.
21. Lund, P.D., et al. (2025). Review of energy system flexibility measures. Renewable and Sustainable Energy Reviews, 185, 113676.
22. Mulleriyawage, U.G.K., et al. (2020). Optimally sizing battery energy storage capacity. Renewable Energy, 148, pp. 1014-1024.
23. NREL (2024). Best Research-Cell Efficiency Chart. Golden, CO: NREL.
24. Obalanlege, M.A., et al. (2020). Performance assessment of hybrid photovoltaic-thermal system. Renewable Energy, 156, pp. 1147-1160.
25. Our World in Data (2024). Solar Energy - Cost and Capacity Trends. https://ourworldindata.org
26. Parida, B., Iniyan, S., and Goic, R. (2011). A review of solar photovoltaic technologies. Renewable and Sustainable Energy Reviews, 15(3), pp. 1625-1636.
27. PV Magazine (2024). Perovskite-silicon tandem solar cells. PV Magazine International, December 2024.
28. PV Tech (2025). Global solar PV surpasses 600 GW annual installations. PV Tech, March 2025.
29. Rai, V. and Robinson, S.A. (2013). Effective information channels for reducing costs. Energy Policy, 62, pp. 320-329.
30. Rawat, P.S., et al. (2024). Design and Performance Analysis of On Grid Solar System. Proceedings of Conference on Power Electronics and Renewable Energy Systems, pp. 112-118.
31. REN21 (2025). Renewables 2025 Global Status Report. Paris: REN21 Secretariat.
32. Rudaw Research Center (2024). Iraq's Electricity Crisis. Erbil: Rudaw Media Network.
33. Serat, Z., et al. (2024). Optimizing renewable energy systems. Journal of Energy Storage, 82, 110534.
34. Shah, K.K., et al. (2015). Assessing the economic viability of residential solar PV. Energy Conversion and Management, 104, pp. 151-158.
35. Shabbir, M., et al. (2017). Battery Size Optimization with Customer PV Installations. IEEE Trans. Industry Applications, 53(1), pp. 294-301.
36. Walker, A. (2013). Solar Energy: Technologies and Project Delivery for Buildings. Hoboken, NJ: Wiley.
37. Worldometers (2024). Iraq CO2 Emissions. https://worldometers.info
38. Zakeri, B. and Syri, S. (2015). Electrical energy storage systems: A comparative life cycle cost analysis. Renewable and Sustainable Energy Reviews, 42, pp. 569-596.
39. Zelazna, A., et al. (2020). A Hybrid vs. On-Grid Photovoltaic System: Multicriteria Analysis. Energies, 13(12), 3978.
