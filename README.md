<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Behar's AP Environmental Review</title>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap');

        :root {
            /* Sleek, updated color palette */
            --primary: #1e293b; /* Slate dark */
            --secondary: #059669; /* Emerald green */
            --accent: #38bdf8; /* Light sky blue for sleek buttons */
            --light-bg: #f8fafc;
            --card-bg: #ffffff;
            --text-main: #334155;
            --text-muted: #64748b;
            --border-color: #e2e8f0;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Inter', sans-serif;
        }

        body {
            background-color: var(--light-bg);
            color: var(--text-main);
            line-height: 1.7;
        }

        /* Hero Banner */
        .hero {
            background: linear-gradient(rgba(30, 41, 59, 0.85), rgba(5, 150, 105, 0.85)), url('https://images.unsplash.com/photo-1511497584788-876760111969?auto=format&fit=crop&q=80&w=2000') center/cover;
            padding: 5rem 2rem;
            text-align: center;
            color: white;
            clip-path: polygon(0 0, 100% 0, 100% 92%, 0 100%);
            margin-bottom: 2rem;
        }

        .hero h1 {
            font-size: 3.8rem;
            margin-bottom: 1rem;
            letter-spacing: 1px;
            text-transform: uppercase;
            text-shadow: 2px 2px 5px rgba(0,0,0,0.4);
        }

        .hero p {
            font-size: 1.3rem;
            max-width: 700px;
            margin: 0 auto 2rem auto;
            opacity: 0.95;
            font-weight: 300;
        }

        .download-btn {
            display: inline-block;
            background-color: var(--accent);
            color: #0f172a;
            padding: 15px 30px;
            font-size: 1.1rem;
            font-weight: 700;
            text-decoration: none;
            border-radius: 50px;
            box-shadow: 0 4px 15px rgba(56, 189, 248, 0.3);
            transition: all 0.3s ease;
        }

        .download-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(56, 189, 248, 0.5);
            background-color: #0ea5e9;
            color: white;
        }

        /* Layout */
        .layout-wrapper {
            display: flex;
            max-width: 1400px;
            margin: 0 auto;
            padding: 0 2rem;
            gap: 2.5rem;
            align-items: flex-start;
        }

        /* Sidebar Navigation */
        .sidebar {
            flex: 0 0 260px;
            background: var(--card-bg);
            padding: 2rem 1.5rem;
            border-radius: 12px;
            box-shadow: 0 10px 25px rgba(0,0,0,0.03);
            position: sticky;
            top: 2rem;
            border: 1px solid var(--border-color);
        }

        .sidebar h3 {
            color: var(--primary);
            margin-bottom: 1.5rem;
            font-size: 1.1rem;
            border-bottom: 2px solid var(--border-color);
            padding-bottom: 10px;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .sidebar nav {
            display: flex;
            flex-direction: column;
            gap: 8px;
        }

        .sidebar a {
            text-decoration: none;
            color: var(--text-muted);
            font-weight: 600;
            padding: 10px 15px;
            border-radius: 8px;
            transition: all 0.2s ease;
            border-left: 4px solid transparent;
            font-size: 0.95rem;
        }

        .sidebar a:hover, .sidebar a.active {
            background-color: #ecfdf5; /* Light emerald */
            color: var(--secondary);
            border-left: 4px solid var(--secondary);
        }

        .sidebar hr {
            border: none;
            border-top: 1px solid var(--border-color);
            margin: 15px 0;
        }

        /* Main Content Area */
        .main-content {
            flex: 1;
            min-width: 0;
        }

        /* Content Cards */
        .content-card {
            background: var(--card-bg);
            border-radius: 12px;
            padding: 3rem;
            margin-bottom: 3rem;
            box-shadow: 0 10px 25px rgba(0,0,0,0.03);
            border-top: 6px solid var(--secondary);
            border-left: 1px solid var(--border-color);
            border-right: 1px solid var(--border-color);
            border-bottom: 1px solid var(--border-color);
        }

        .unit-header {
            display: flex;
            align-items: center;
            gap: 15px;
            margin-bottom: 2rem;
            border-bottom: 2px solid var(--border-color);
            padding-bottom: 1.5rem;
        }

        .unit-header i {
            font-size: 2.2rem;
            color: var(--secondary);
        }

        .unit-header h2 {
            font-size: 2rem;
            color: var(--primary);
            letter-spacing: -0.5px;
        }

        /* Text formatting */
        .content-card h3 {
            color: var(--secondary);
            font-size: 1.4rem;
            margin: 2rem 0 1rem 0;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .content-card h3::before {
            content: '';
            display: block;
            width: 8px;
            height: 20px;
            background-color: var(--accent);
            border-radius: 4px;
        }

        .content-card p {
            margin-bottom: 1rem;
            color: var(--text-main);
        }

        .content-card ul {
            margin-left: 2rem;
            margin-bottom: 1.5rem;
            color: var(--text-main);
        }

        .content-card li {
            margin-bottom: 0.5rem;
        }

        .highlight-box {
            background: #f1f5f9;
            border-left: 4px solid var(--secondary);
            padding: 1.5rem;
            margin: 1.5rem 0;
            border-radius: 0 8px 8px 0;
            color: var(--text-main);
        }

        .highlight-box strong {
            color: var(--primary);
        }

        /* Specific Section Styles */
        .btn-outline {
            display: inline-block;
            border: 2px solid var(--secondary);
            color: var(--secondary);
            padding: 10px 20px;
            border-radius: 8px;
            text-decoration: none;
            font-weight: 600;
            transition: all 0.3s ease;
            margin-top: 10px;
        }

        .btn-outline:hover {
            background-color: var(--secondary);
            color: white;
        }

        .video-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }

        .video-card {
            background: var(--light-bg);
            padding: 20px;
            border-radius: 12px;
            border: 1px solid var(--border-color);
            text-align: center;
        }

        .video-card i {
            font-size: 3rem;
            color: #ef4444; /* YouTube Red */
            margin-bottom: 15px;
        }

        .about-grid {
            display: flex;
            gap: 30px;
            align-items: center;
        }

        .about-image {
            width: 150px;
            height: 150px;
            background-color: var(--secondary);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 4rem;
            flex-shrink: 0;
            box-shadow: 0 10px 20px rgba(5, 150, 105, 0.2);
        }

        footer {
            background-color: var(--primary);
            color: white;
            text-align: center;
            padding: 3rem;
            margin-top: 4rem;
        }

        /* Responsive */
        @media (max-width: 900px) {
            .layout-wrapper {
                flex-direction: column;
            }
            .sidebar {
                position: static;
                width: 100%;
                margin-bottom: 2rem;
            }
            .hero h1 { font-size: 2.5rem; }
            .about-grid { flex-direction: column; text-align: center; }
        }
    </style>
</head>
<body>

    <header class="hero">
        <h1>Behar's AP Environmental Review</h1>
        <p>The Sleek & Ultimate Master Study Guide • Units 1-8</p>
        
        <a href="The Ultimate AP Environmental Science Master Study Guide.pdf" download="The Ultimate AP Environmental Science Master Study Guide.pdf" class="download-btn">
            <i class="fas fa-file-download"></i> Here's a more in-depth study guide!
        </a>
    </header>

    <div class="layout-wrapper">
        
        <aside class="sidebar">
            <h3>Course Navigation</h3>
            <nav id="navbar">
                <a href="#unit1" class="active">Unit 1: Ecosystems</a>
                <a href="#unit2">Unit 2: Biodiversity</a>
                <a href="#unit3">Unit 3: Populations</a>
                <a href="#unit4">Unit 4: Earth Systems</a>
                <a href="#unit5">Unit 5: Land & Water</a>
                <a href="#unit6">Unit 6: Energy</a>
                <a href="#unit7">Unit 7: Atmosphere</a>
                <a href="#unit8">Unit 8: Pollution</a>
                <hr>
                <a href="#exam-info"><i class="fas fa-calendar-check"></i> Exam Info</a>
                <a href="#videos"><i class="fab fa-youtube"></i> Study Videos</a>
                <a href="#about"><i class="fas fa-user-circle"></i> About Behar</a>
            </nav>
        </aside>

        <main class="main-content">

            <section id="unit1" class="content-card">
                <div class="unit-header">
                    <i class="fas fa-tree"></i>
                    <h2>Unit 1: The Living World: Ecosystems</h2>
                </div>
                
                <h3>1.1 Ecosystems & Symbiosis</h3>
                <p>Ecosystems result from complex interactions between biotic (living) communities and their abiotic (non-living) physical environments.</p>
                <ul>
                    <li><strong>Mutualism (+/+):</strong> Both organisms benefit. Example: Mycorrhizal fungi attach to plant roots; the fungi increase water/nutrient absorption, while the plant provides carbohydrates.</li>
                    <li><strong>Commensalism (+/0):</strong> One benefits, the other is unaffected. Example: Epiphytic orchids growing on the high branches of tropical trees to access sunlight.</li>
                    <li><strong>Parasitism (+/-):</strong> One benefits, one is harmed. Example: Sea lampreys attaching to lake trout, draining their fluids.</li>
                    <li><strong>Resource Partitioning:</strong> To avoid competitive exclusion (where one species outcompetes another), species divide niches. Example: warblers foraging in different specific sections of the same spruce tree.</li>
                </ul>

                <h3>1.2 & 1.3 Terrestrial and Aquatic Biomes</h3>
                <p>Biomes are geographic regions characterized by distinct climate patterns and specific plant/animal communities.</p>
                <ul>
                    <li><strong>Tropical Rainforest:</strong> High temp/precipitation. Nutrient-poor soil due to rapid decomposition. Highest terrestrial biodiversity.</li>
                    <li><strong>Taiga (Boreal Forest):</strong> Cold, moderate precipitation. Coniferous trees. Slow decomposition leads to nutrient-dense but highly acidic soil (pine needles).</li>
                    <li><strong>Tundra:</strong> Extremely cold, permafrost prevents deep root growth and traps massive amounts of methane/carbon.</li>
                    <li><strong>Estuaries/Salt Marshes:</strong> Brackish water where rivers meet oceans. Critical nursery for marine life; filters water pollutants. Extremely high primary productivity.</li>
                    <li><strong>Open Ocean:</strong> Low productivity per square meter, but its sheer vastness makes it the largest carbon sink and highest overall contributor to primary productivity.</li>
                </ul>

                <h3>1.4 - 1.7 Biogeochemical Cycles</h3>
                <p><strong>The Carbon Cycle:</strong> Ocean is the largest sink. Photosynthesis removes CO2; Respiration, Decomposition, and Combustion (burning fossil fuels) add CO2 to the atmosphere.</p>
                <div class="highlight-box">
                    <strong>The Nitrogen Cycle Steps:</strong><br>
                    1. Fixation (N2 to Ammonia via bacteria/lightning) <br>
                    2. Nitrification (Ammonia to Nitrites to Nitrates) <br>
                    3. Assimilation (Plants absorb Nitrates) <br>
                    4. Ammonification (Decomposers return N to soil) <br>
                    5. Denitrification (Anaerobic bacteria return N2 to atmosphere).
                </div>
                <p><strong>The Phosphorus Cycle:</strong> Has NO atmospheric phase. It is entirely sedimentary and driven by geologic weathering. Because it is incredibly slow to replenish, it is often the limiting factor for plant growth.</p>

                <h3>1.8 - 1.11 Energy Flow & Primary Productivity</h3>
                <ul>
                    <li><strong>GPP (Gross Primary Productivity):</strong> Total solar energy captured by producers.</li>
                    <li><strong>NPP (Net Primary Productivity):</strong> The energy captured minus the energy producers use for cellular respiration. This is the actual biomass available to consumers.</li>
                    <li><strong>The 10% Rule:</strong> Based on the Second Law of Thermodynamics (entropy). When energy transfers trophic levels, ~90% is lost as heat. Only ~10% is converted into consumer biomass.</li>
                    <li><strong>Trophic Cascade:</strong> Removing a keystone species (like the Yellowstone Gray Wolf) causes secondary consumers to overpopulate, decimating producers and altering the physical ecosystem.</li>
                </ul>
            </section>

            <section id="unit2" class="content-card">
                <div class="unit-header">
                    <i class="fas fa-paw"></i>
                    <h2>Unit 2: The Living World: Biodiversity</h2>
                </div>

                <h3>2.1 Biodiversity Scales & 2.2 Ecosystem Services</h3>
                <p>Biodiversity is assessed at three scales: Genetic (variety of DNA, prevents inbreeding depression), Species (richness and evenness), and Habitat (variety of biomes).</p>
                <ul>
                    <li><strong>Provisioning Services:</strong> Goods we harvest directly (timber, fish, fresh water).</li>
                    <li><strong>Regulating Services:</strong> Processes that moderate natural phenomena (wetlands absorbing floods, forests sequestering carbon).</li>
                    <li><strong>Cultural Services:</strong> Non-material benefits (recreation, ecotourism).</li>
                    <li><strong>Supporting Services:</strong> Foundational processes (photosynthesis, nutrient cycling, soil formation).</li>
                </ul>

                <h3>2.3 Island Biogeography</h3>
                <div class="highlight-box">
                    <strong>The Two Rules of Island Biogeography:</strong><br>
                    1. <strong>Size:</strong> Larger islands have higher biodiversity (more varied habitats, lower extinction rates).<br>
                    2. <strong>Distance:</strong> Islands closer to the mainland have higher biodiversity (higher rates of immigration/colonization).<br>
                    <em>Note: This also applies to "habitat islands" like national parks surrounded by cities!</em>
                </div>

                <h3>2.4 Ecological Tolerance & 2.5 Natural Disruptions</h3>
                <p>Every species has an <strong>Optimum Range</strong> (where it thrives), a <strong>Zone of Physiological Stress</strong> (survives but stunted), and a <strong>Zone of Intolerance</strong> (death) for abiotic conditions like pH and temperature.</p>
                <p>Earth's climate naturally shifts over geologic time due to Milankovitch cycles, volcanoes, and tectonics. Rapid anthropogenic (human-caused) changes often outpace evolutionary adaptation, leading to extinction.</p>

                <h3>2.7 Ecological Succession</h3>
                <ul>
                    <li><strong>Primary Succession:</strong> Occurs in a lifeless area with NO soil (new volcanic island). Pioneer species like lichens and mosses chemically weather rock to form primitive soil.</li>
                    <li><strong>Secondary Succession:</strong> Occurs where an ecosystem was destroyed but soil remains intact (after a forest fire). Fast-growing grasses ➔ Shrubs ➔ Pines ➔ Hardwood climax community.</li>
                </ul>
            </section>

            <section id="unit3" class="content-card">
                <div class="unit-header">
                    <i class="fas fa-users"></i>
                    <h2>Unit 3: Populations</h2>
                </div>

                <h3>3.1 - 3.3 Species Strategies & Survivorship</h3>
                <ul>
                    <li><strong>Generalists vs Specialists:</strong> Generalists (raccoons) have broad niches and adapt easily. Specialists (pandas) have narrow niches and are highly prone to extinction.</li>
                    <li><strong>K-Selected:</strong> Large size, long lifespan, few offspring, heavy parental care (Humans, elephants). Stabilize near carrying capacity. Show Type I survivorship curve.</li>
                    <li><strong>r-Selected:</strong> Small size, short lifespan, massive amounts of offspring, zero parental care. Opportunistic rapid growth (Mosquitoes). Show Type III survivorship curve.</li>
                </ul>

                <h3>3.4 Carrying Capacity (K)</h3>
                <p>The maximum population size an environment can sustainably support. If a population grows exponentially and exceeds K, an <strong>Overshoot</strong> occurs, exhausting resources. This inevitably leads to a massive population crash known as a <strong>Dieback</strong>.</p>

                <h3>3.6 - 3.9 Human Demography & DTM</h3>
                <p><strong>Age Structure Diagrams:</strong> A broad base indicates rapid future growth (Nigeria). A column shape indicates stable growth (USA). An inverted pyramid indicates a shrinking, aging population (Japan).</p>
                <p><strong>Total Fertility Rate (TFR):</strong> TFR drops with women's education, access to contraceptives, delayed marriage, and urbanization.</p>
                
                <div class="highlight-box">
                    <strong>The Demographic Transition Model (DTM):</strong><br>
                    <strong>Stage 1:</strong> High birth & death rates. Small stable population.<br>
                    <strong>Stage 2:</strong> Death rates fall rapidly (medicine, sanitation). Explosive exponential growth.<br>
                    <strong>Stage 3:</strong> Birth rates fall (education, economy). Growth slows down.<br>
                    <strong>Stage 4:</strong> Low birth & death rates. Population is stable or declining.
                </div>
            </section>

            <section id="unit4" class="content-card">
                <div class="unit-header">
                    <i class="fas fa-globe-americas"></i>
                    <h2>Unit 4: Earth Systems & Resources</h2>
                </div>

                <h3>4.1 Plate Tectonics</h3>
                <p>The Earth's crust (lithosphere) floats on the semi-molten asthenosphere.</p>
                <ul>
                    <li><strong>Divergent:</strong> Plates pull apart. Magma rises to create new crust (Mid-ocean ridges, seafloor spreading).</li>
                    <li><strong>Convergent:</strong> Plates crash. Subduction creates coastal mountains/volcanoes. Continental crashes fold into massive mountains (Himalayas).</li>
                    <li><strong>Transform:</strong> Plates slide past each other. Friction releases as earthquakes (San Andreas Fault).</li>
                </ul>

                <h3>4.2 & 4.3 Soil Formation and Properties</h3>
                <p><strong>Soil Horizons:</strong> O (Organic leaf litter) ➔ A (Topsoil, rich) ➔ E (Leaching zone) ➔ B (Subsoil, clays) ➔ C (Weathered rock) ➔ R (Bedrock).</p>
                <p><strong>Properties:</strong> Sand has high porosity/permeability (water drains fast). Clay has low permeability but high Cation Exchange Capacity (CEC) to hold nutrients. <strong>Loam</strong> is the perfect agricultural mix of sand, silt, and clay.</p>

                <h3>4.4 - 4.8 Atmosphere, Winds, and Climate</h3>
                <ul>
                    <li><strong>Troposphere vs Stratosphere:</strong> Troposphere is where we live and weather occurs. The Stratosphere contains the protective ozone layer (O3) which absorbs UV radiation.</li>
                    <li><strong>Coriolis Effect & Convection:</strong> Warm air rises at the equator (creating wet rainforests) and sinks at 30° latitude (creating major deserts). Earth's rotation deflects these winds.</li>
                    <li><strong>Seasons:</strong> Caused entirely by the 23.5° tilt of Earth's axis altering the angle of Insolation (incoming solar radiation), NOT the distance from the sun.</li>
                </ul>
                <div class="highlight-box">
                    <strong>The Rain Shadow Effect:</strong> Prevailing winds force warm, moist air up a mountain. It cools and rains on the windward side. The completely dry air sinks down the leeward side, creating a desert.
                </div>

                <h3>4.9 El Niño and La Niña (ENSO)</h3>
                <p><strong>Normal:</strong> Trade winds blow west. Cold, nutrient-rich water rises off South America (Upwelling), creating massive fisheries.</p>
                <p><strong>El Niño:</strong> Trade winds weaken. Warm water sloshes back to South America, stopping upwelling. Fisheries collapse, and global weather is severely altered (floods in US, drought in Australia).</p>
            </section>

            <section id="unit5" class="content-card">
                <div class="unit-header">
                    <i class="fas fa-tractor"></i>
                    <h2>Unit 5: Land & Water Use</h2>
                </div>

                <h3>5.1 Tragedy of the Commons</h3>
                <p>When individuals act in self-interest to exploit an unregulated, shared resource (like open-ocean fishing or public grazing land), they deplete and destroy it for everyone. Managed via strict quotas or private ownership.</p>

                <h3>5.3 The Green Revolution & 5.4 Agricultural Impacts</h3>
                <p>The transition to industrial corporate farming via mechanization, GMOs, agrochemicals, and monocropping. </p>
                <ul>
                    <li><strong>Tilling:</strong> Turning soil kills weeds but massively increases erosion and releases stored soil carbon.</li>
                    <li><strong>Salinization:</strong> Irrigation water evaporates in dry climates, leaving trace salts behind until the soil becomes too toxic for crops.</li>
                    <li><strong>Pesticide Treadmill:</strong> Pests evolve resistance, forcing farmers to use increasingly toxic chemical sprays.</li>
                </ul>

                <h3>5.7 Meat Production & 5.8 Overfishing</h3>
                <p><strong>CAFOs (Feedlots):</strong> High efficiency, but animals are prone to disease requiring heavy antibiotics. Creates massive "manure lagoons" that leak into groundwater.</p>
                <p><strong>Overfishing:</strong> Leads to fishery collapse and severe "bycatch" (the unintentional killing of non-target species like dolphins and sea turtles in massive nets).</p>

                <h3>5.10 Urbanization & 5.15 Sustainable Agriculture</h3>
                <p><strong>Impervious Surfaces:</strong> Asphalt prevents water infiltration, rushing polluted runoff into storm drains and causing flash floods. Mitigated by permeable pavement and green roofs.</p>
                <div class="highlight-box">
                    <strong>Sustainable Solutions:</strong><br>
                    <strong>IPM:</strong> Using biological controls (ladybugs) and physical barriers first; chemicals are an absolute last resort.<br>
                    <strong>Soil Conservation:</strong> Contour plowing, terracing, windbreaks, and no-till agriculture preserve topsoil.<br>
                    <strong>Crop Rotation:</strong> Planting legumes (soybeans) naturally replenishes soil nitrogen without synthetic fertilizers.
                </div>
            </section>

            <section id="unit6" class="content-card">
                <div class="unit-header">
                    <i class="fas fa-bolt"></i>
                    <h2>Unit 6: Energy Resources & Consumption</h2>
                </div>

                <h3>6.1 - 6.5 Fossil Fuels</h3>
                <p>As nations industrialize, they transition from biomass (wood/dung) to fossil fuels. The standard electricity generation process: Burn fuel ➔ Heat boils water ➔ Steam turns turbine ➔ Turbine spins generator.</p>
                <ul>
                    <li><strong>Coal:</strong> Dirtiest fossil fuel (high SO2 and toxic metals).</li>
                    <li><strong>Natural Gas:</strong> "Cleanest" fossil fuel (least CO2), but extracted via fracking, which causes severe groundwater contamination risks and methane leaks.</li>
                </ul>

                <h3>6.6 Nuclear Power</h3>
                <p>Generates massive energy via fission (splitting Uranium-235 atoms). </p>
                <p><strong>Pros:</strong> Emits absolutely NO air pollution or CO2 during regular operation.</p>
                <p><strong>Cons:</strong> Leaves behind highly radioactive spent fuel rods that require secure long-term storage for thousands of years. Risk of catastrophic meltdowns (Chernobyl).</p>

                <h3>6.7 - 6.12 Renewable Energy</h3>
                <ul>
                    <li><strong>Biomass/Ethanol:</strong> Burning "modern carbon" doesn't add net new CO2 to the atmosphere, but overharvesting causes deforestation.</li>
                    <li><strong>Solar (PV Cells):</strong> Converts sunlight directly to electricity. Clean, but intermittent and requires toxic mining for rare earth metals.</li>
                    <li><strong>Hydroelectric:</strong> Reliable and clean, but massive dams cause habitat flooding, prevent fish migration (salmon), and stagnant reservoirs release methane.</li>
                    <li><strong>Wind:</strong> Kinetic energy spins turbines. Offshore farms are highly consistent. Cons: Bird/bat mortality and aesthetic (NIMBY) complaints.</li>
                    <li><strong>Hydrogen Fuel Cell:</strong> Highly efficient vehicle power where the only emission is pure water (H2O). However, pure hydrogen must be separated using fossil fuel energy.</li>
                </ul>
            </section>

            <section id="unit7" class="content-card">
                <div class="unit-header">
                    <i class="fas fa-smog"></i>
                    <h2>Unit 7: Atmospheric Pollution</h2>
                </div>

                <h3>7.1 Primary vs Secondary Pollutants</h3>
                <p><strong>Primary:</strong> Emitted straight from the source (CO, SO2, NOx, Particulate Matter).</p>
                <p><strong>Secondary:</strong> Formed via atmospheric reactions with sunlight or water (Ozone, Sulfuric Acid).</p>
                <p><em>The Clean Air Act limits the 6 criteria pollutants: NOSCLP (Nitrogen oxides, Ozone, Sulfur dioxide, Carbon monoxide, Lead, Particulate Matter).</em></p>

                <h3>7.2 Photochemical Smog & 7.3 Thermal Inversions</h3>
                <div class="highlight-box">
                    <strong>Photochemical Smog Recipe:</strong><br>
                    NOx (from car exhaust) + VOCs (gasoline fumes/paints) + Heat + Sunlight = <strong>Tropospheric (Ground-Level) Ozone</strong>.
                </div>
                <p><strong>Thermal Inversion:</strong> Normally, warm polluted air rises and disperses. An inversion occurs when a layer of warm air traps cold, polluted air near the ground. Common in valley cities (Los Angeles, Mexico City), trapping smog directly over the population.</p>

                <h3>7.5 Indoor Air Pollutants</h3>
                <ul>
                    <li><strong>Developing Nations:</strong> Highest risk is burning biomass/coal indoors with poor ventilation, exposing families to severe Particulate Matter and CO.</li>
                    <li><strong>Developed Nations:</strong> Tight sealed homes trap Asbestos (insulation, causes mesothelioma), Radon-222 (radioactive gas from bedrock, #2 cause of lung cancer), and VOCs (formaldehyde in furniture).</li>
                </ul>

                <h3>7.6 Reduction & 7.7 Acid Rain</h3>
                <p>Acid rain is caused by SO2 (coal plants) and NOx (cars) reacting with water vapor. It lowers lake pH and leaches toxic heavy metals from soil.</p>
                <p><strong>Mitigation Technology:</strong> Catalytic converters on car exhausts, and Wet/Dry Scrubbers inside factory smokestacks to capture pollutants before they enter the air.</p>
            </section>

            <section id="unit8" class="content-card">
                <div class="unit-header">
                    <i class="fas fa-water"></i>
                    <h2>Unit 8: Aquatic & Terrestrial Pollution</h2>
                </div>

                <h3>8.1 Point vs Nonpoint Source & 8.3 Endocrine Disruptors</h3>
                <p><strong>Point Source:</strong> Identifiable (factory pipe). <strong>Nonpoint Source:</strong> Diffuse (agricultural runoff, city streets).</p>
                <p><strong>Endocrine Disruptors:</strong> Synthetic chemicals (BPA, phthalates, atrazine) that mimic or block hormones. They cause severe developmental defects and gender imbalances in amphibians and fish.</p>

                <h3>8.5 Eutrophication</h3>
                <div class="highlight-box">
                    <strong>The Steps to a Dead Zone:</strong><br>
                    1. Excess nutrients (nitrogen/phosphorus from fertilizer) enter water.<br>
                    2. Rapid Algal Bloom occurs on the surface.<br>
                    3. Thick algae blocks sunlight; aquatic plants below die.<br>
                    4. Algae run out of nutrients and die.<br>
                    5. Aerobic bacteria aggressively decompose the dead algae, consuming massive amounts of Dissolved Oxygen (DO).<br>
                    6. The water becomes <strong>hypoxic</strong>, creating a Dead Zone where fish suffocate.
                </div>

                <h3>8.7 POPs & 8.8 Biomagnification</h3>
                <p><strong>POPs (Persistent Organic Pollutants):</strong> Synthetic chemicals (like DDT) that do not break down, are fat-soluble, and travel long distances via wind/water.</p>
                <ul>
                    <li><strong>Bioaccumulation:</strong> Toxins building up in a <em>single</em> organism's fat tissue over its lifetime.</li>
                    <li><strong>Biomagnification:</strong> Toxins increasing in concentration as they move <em>up</em> the food chain. Apex predators (like Bald Eagles) suffer the most severe toxic effects.</li>
                </ul>

                <h3>8.9 Solid Waste & 8.11 Sewage Treatment</h3>
                <p><strong>Sanitary Landfills:</strong> Highly engineered with clay/plastic bottom liners, leachate collection pipes to prevent groundwater contamination, and methane recovery systems.</p>
                <p><strong>Sewage Treatment Steps:</strong></p>
                <ol style="margin-left: 2rem;">
                    <li><strong>Primary (Physical):</strong> Screens and settling tanks remove solid grit/plastics.</li>
                    <li><strong>Secondary (Biological):</strong> Aerobic bacteria are added to break down dissolved organic waste.</li>
                    <li><strong>Tertiary (Chemical):</strong> Advanced removal of nitrogen and phosphorus.</li>
                    <li><strong>Disinfection:</strong> UV light, ozone, or chlorine kills remaining pathogens before discharge.</li>
                </ol>
            </section>

            <section id="exam-info" class="content-card">
                <div class="unit-header">
                    <i class="fas fa-calendar-check"></i>
                    <h2>College Board & Exam Info</h2>
                </div>
                <p>The AP Environmental Science Exam is usually administered in early May. Being prepared for the format is half the battle!</p>
                
                <div class="highlight-box">
                    <strong>The Exam Format:</strong><br>
                    <ul>
                        <li><strong>Section I: Multiple Choice</strong> - 80 Questions (90 Minutes). 60% of Exam Score.</li>
                        <li><strong>Section II: Free Response (FRQ)</strong> - 3 Questions (70 Minutes). 40% of Exam Score.
                            <br><em>Includes 1 Design an Investigation, 1 Analyze an Environmental Problem, and 1 Analyze an Environmental Problem with Math.</em>
                        </li>
                    </ul>
                </div>
                
                <p>Be sure to check your specific testing date and get official practice resources directly from the College Board.</p>
                <a href="https://apstudents.collegeboard.org/courses/ap-environmental-science" target="_blank" class="btn-outline">
                    <i class="fas fa-external-link-alt"></i> Visit Official APES College Board Page
                </a>
            </section>

            <section id="videos" class="content-card">
                <div class="unit-header">
                    <i class="fab fa-youtube"></i>
                    <h2>Top Study Videos</h2>
                </div>
                <p>Need a visual breakdown? These are the absolute best YouTube channels for reviewing AP Environmental Science concepts.</p>
                
                <div class="video-grid">
                    <div class="video-card">
                        <i class="fab fa-youtube"></i>
                        <h3>Mr. Smedes</h3>
                        <p>Incredible unit reviews, FRQ tips, and comprehensive exam prep dedicated purely to APES.</p>
                        <a href="https://www.youtube.com/@Smedes" target="_blank" class="btn-outline">Watch Channel</a>
                    </div>
                    <div class="video-card">
                        <i class="fab fa-youtube"></i>
                        <h3>Bozeman Science</h3>
                        <p>Paul Andersen's classic videos break down the complex science, math, and cycles of APES.</p>
                        <a href="https://www.youtube.com/playlist?list=PLllVwaZQkS2qK4Z6xBVPTwsywGWxuSFCZ" target="_blank" class="btn-outline">Watch Playlist</a>
                    </div>
                </div>
            </section>

            <section id="about" class="content-card">
                <div class="unit-header">
                    <i class="fas fa-user-circle"></i>
                    <h2>About Behar Berisha</h2>
                </div>
                
                <div class="about-grid">
                    <div class="about-image">
                        <i class="fas fa-user-graduate"></i>
                    </div>
                    <div>
                        <h3>Creator of the Master Study Guide</h3>
                        <p>Hi, I'm Behar Berisha! I am a proud student at Newtown High School in Elmhurst, NY, and the creator of this AP Environmental Science Study Hub. </p>
                        <p>I am deeply passionate about STEM, civic engagement, and politics. As a state champion debater and participant in the National Harvard Debate Tournament, I love researching, communicating complex ideas, and advocating for what matters. In fact, my passion for education led me to directly advocate for and successfully help create a brand new AP Chemistry course at my school so my peers and I could have better STEM opportunities!</p>
                        <p>As a member of the National Honor Society, I approach all my academic and community commitments—from participating in various clubs to writing a developing biography—with a strong sense of responsibility and leadership. I built this website and the accompanying study guide to help both myself and my fellow students master APES and crush the exam.</p>
                    </div>
                </div>
            </section>

        </main>
    </div>

    <footer>
        <h2>Built for a 5! 🌲</h2>
        <p>Created by Behar Berisha | Newtown High School</p>
    </footer>

    <script>
        // Smooth scrolling and active state update for the sidebar
        const sections = document.querySelectorAll('.content-card');
        const navLinks = document.querySelectorAll('.sidebar nav a');

        window.addEventListener('scroll', () => {
            let current = '';
            sections.forEach(section => {
                const sectionTop = section.offsetTop;
                if (pageYOffset >= (sectionTop - 150)) {
                    current = section.getAttribute('id');
                }
            });

            navLinks.forEach(link => {
                link.classList.remove('active');
                if (link.getAttribute('href').includes(current)) {
                    link.classList.add('active');
                }
            });
        });

        // Smooth scroll click
        navLinks.forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                const targetId = this.getAttribute('href');
                const targetSection = document.querySelector(targetId);
                
                window.scrollTo({
                    top: targetSection.offsetTop - 30, // Slight offset for visual comfort
                    behavior: 'smooth'
                });
            });
        });
    </script>
</body>
</html>
