# My Research and What Problems to Confront

## Mixing

First problem was mixing. Fresh fuel and air only get a split second before the wave comes back around so they gotta blend almost instantly or the wave goes patchy which obviously can cause issues like more vibrations and a more so (already) unstable shockwave. Real RDEs shoot the fuel and air jets across each other (**jet in crossflow**) instead of side by side, the crash makes vortices that stir the fuel into the air. Smaller holes push the fuel deeper into the air and theres a sweet spot for how many fuel holes you want. Worse mixing means a weaker wave, slower and less efficient with less pressure gain. Even good designs dont fully solve it. Most of this is hydrogen-air simulation and lab bullshit so not real jet fuel. Ironic for a jet engine.

My Sources:

[Sato, Van Beck, Raman (2023), Frontiers in Aerospace Engineering](https://www.frontiersin.org/journals/aerospace-engineering/articles/10.3389/fpace.2023.1123249/full)

[Raj, Meadows (2024), Influence of fuel inhomogeneity on detonation wave propagation in a rotating detonation combustor](https://vtechworks.lib.vt.edu/items/bf329c33-07bd-4085-ae39-12a94adccbbe)

[Rahman et al. (2021), Predictive Numerical Analysis on the Mixing Characteristics in a Rotating Detonation Engine (RDE), EVERGREEN](https://www.tj.kyushu-u.ac.jp/evergreen/contents/EG2021-8_1_content/123-130.html)

[RDE mixing and injection flow field study, via Peeref](https://peeref.com/works/2415878)

[14-Nov-2026]




## Heat

Second problem is heat. Detonation hits the walls way harder than a normal flame and the wave sweeps past THOUSANDS of times a second, so the walls overheat unless they get cooled **HARD**. My idea was the old petrol and LPG trick, run the fuel through the walls first so it soaks up the heat and then inject it. Turns out thats a real thing called **regenerative cooling** and the hot fuel flash vaporizes at the inlet which helps the mixing too. NASA has fired rocket versions of it. BUT. Yes but the catch is the cooling channels get shaken by the detonation and can fail from fatigue. Also just to note so that my thought process is out there. Had a thought of water injection (the BMW way) for the worst hot spots, not applying it to the design. Turns out to be a shitty idea for something of this caliber.

My Sources:

[RTX patent, Regenerative cooling and adjustable throat for rotating detonation engine](https://patents.justia.com/patent/20240077028)

[NASA NTRS, Final Report for ECI RDRE (rotating detonation rocket engine)](https://ntrs.nasa.gov/api/citations/20240013951/downloads/Final%20Report%20for%20ECI%20RDRE%20Open%20Release%20Final%20v2.pdf)

[MIT DSpace, cooling channel fatigue under detonation loading in RDREs](https://dspace.mit.edu/handle/1721.1/143397)

[USPTO patent, Film cooling with rotating detonation engine to secondary combustion (water injection)](https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/11840988)

[14-Nov-2026]




## Messy exhaust

Third problem is the exhaust. A turbine always wants a calm steady flow and an RDE spits out the opposite, transonic (anything going roughly mach 0.8 to 1.2) flow is full of shocks that spin around at a few to TENS of kilohertz. Basically a pulsing fire hose swirling sideways at the blades. Fix number one is a **diffuser** between the ring and the turbine, same idea as when I looked into RamJets, the wide space slows the flow down. It killed the angled shock and the sideways swirl, but the axial speed still swung between 300 and 1200 m/s soooo its clearly not perfect. Bigger issue is shocks bouncing off the hardware downstream and travelling back into the ring, which can mess with the wave badly potentially fucking it up and breaking the rhythm. My sources say to shape the combustor and the duct to deal with that, and another option is a turbine built to take supersonic flow (**supersonic inlet turbine**). My call for the design is diffuser, shaped transition duct, turbine and then an **aerospike** at the back as the final nozzle (absolute freak for em). NASA has hot fired aerospike RDEs and Purdue/NASA tested them against nozzleless ones, but those are rockets, so I still gotta check how it works with a turbine in front of it. Also aerospike should make fewer shock diamonds but I doubt they fully go away with RDE exhaust.

My Sources:

[Agrawal, Meadows (2022), UTSR Project Review, Integrating a Rotating Detonation Combustor with a Power Generating Gas Turbine](https://netl.doe.gov/sites/default/files/netl-file/22UTSR_Agrawal.pdf)

[Aero-Thermal Characterization of Accelerating and Diffusing Passages Downstream of Rotating Detonation Combustors, OSTI](https://www.osti.gov/biblio/2499549)

[Talukdar et al., Diffuser Integration With a Rotating Detonation Combustor for Power Generating Gas Turbines, ASME Turbo Expo poster](https://asme-turboexpo.secure-platform.com/a/solicitations/243/sessiongallery/20429/application/162889)

[Supersonic inlet turbine design limits for rotating detonation combustors, Politecnico di Milano](https://re.public.polimi.it/retrieve/639e97f9-7a12-4b3b-8461-37f6500c6349/finalPaper_ETC_print.pdf)

[Harroun, Heister, Ruf, Experimental Validation of Nozzle Flow Simulations for Rotating Detonation Rocket Engines, NASA NTRS](https://ntrs.nasa.gov/citations/20230009329)

[15-Nov-2026]
