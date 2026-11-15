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

Update: this was written for the turbine route when I was still caught in pure chain of thought. Went rocket instead so the diffuser, duct and turbine stuff is dead. The shocks bouncing back into the ring and the aerospike still count. Ugh fuck. 

[15-Nov-2026]



##  Start and stability

Fourth problem is getting it started and keeping the wave alive. Starting is the hard part cus its a COLD start, same reason a cold diesel needs glow plugs. It also screws with my regenerative cooling idea since cold walls cant soak up any heat yet, so the fuel goes in cold and mixes like shit. Real engines light it with a **pre-detonator**, a small tube stuck on the side of the ring where a detonation forms first and then shoots into the chamber. Basically a pulsejet mounted facing the walls. Where you put it and how much energy it has changes how the wave starts, even which way it spins. My idea is to pulse it a few times to warm the walls and let the supply pressure build before the wave catches.

Stability is allll about the refill. The number of waves depends on how much air is flowing, more air tends to mean more waves (and space too), and if the supply drops hard the wave count drops with it. During startup it can even go from 1 wave to 2 all by itself. Weaker secondary waves can also show up and mess with the main ones. One wave only acts like a vibration motor you'd find in a PS4 controller, one big kick per lap so in such I want **several waves** cus I like insanity and its smoother. BUT. Yes but the cost is each wave needs its own fresh mix, so the compressor and injectors gotta push enough flow to keep that wave count stable which means more overall consumption but hey if this goes anywhere and some thirsty headhunter wants it I won't be the one covering billing. Hopefully.

My Sources:

[Mode-Locked Rotating Detonation Waves: Experiments and a Model Equation, arXiv](https://arxiv.org/pdf/1908.03116)

[Effects of Inlet Condition Variations on the Operating Modes of Rotating Detonation Engines, DOAJ](https://doaj.org/article/48889e630674420e9a87c6502a82fcd8)

[Han et al. (2026), Effects of ignition conditions on detonation wave evolution in a rotating detonation engine, BIT](https://pure.bit.edu.cn/en/publications/effects-of-ignition-conditions-on-detonation-wave-evolution-in-a-/)

[Pre-detonator design and testing for rotating detonation combustors, Springer (CEAS Space Journal)](https://link.springer.com/article/10.1007/s12567-025-00605-y)

[Wang, Qiao, Le (2021), Combustion Characteristics in Rotating Detonation Engines, International Journal of Aerospace Engineering](https://doaj.org/article/a777536c82bc4922b73d1e32f6f0f866)

[Ullman, Raman (2024), Influence of injector configuration on secondary wave formation and propagation in a rotating detonation combustor](https://doaj.org/article/3d620933278d46bebdb621a02673c47e)

[15-Nov-2026]



## Vibration

Fifth problem is vibration and its a **BIG** one. The wave hits the walls thousands of times (like 1-10 kHz holy fuck) a second so everything gets kicked at a fixed rhythm. and like I said one wave only is like a vibration motor, one big kick per lap, so several waves smooth it out. The real danger is **resonance**. Every part rings at its own pitch like a wine glass or harmonics in a guitar, and if the wave rhythm lands near that pitch the part shakes WAY harder than the detonation alone would make it. And the wave pitch isnt fixed, it moves with the wave count (few to tens of kilohertz) and with the heat, so one tuned fix wont cover it. Gas turbine combustors already use **Helmholtz resonators** for this (a hollow cavity on a narrow neck tuned to one pitch, kinda like a bottle) and theres even a patent for RDE liners with a few different resonators mixed in rows. My idea is a ring of **quarter-wave cavities** machined straight into the outer wall at different depths so they cover a few pitches, plus **choked injectors** so the refill stays steady and the chamber pressure swings cant shove back into the supply. Though there are some catches:
Cavities fight the regenerative cooling channels for wall space, and a choked injector burns some of the pressure gain, so the compressor has to push harder. Thats fine though because we only need around 12:1 and modern big engines go way past that (like 60:1), plus RDEs gain the most at low pressure ratios. Gotta find a proper source for the choked injector and quarter-wave bits cus right now thats my own thinking.

My Sources:

[Acoustically absorptive liners for passive control of unwanted acoustic modes in rotating detonation combustors, USPTO patent US12234773](https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/12234773)

[Apparatus for damping acoustic vibrations in a combustor (Helmholtz resonator), USPTO patent US6634457](https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/6634457)

[Aero-Thermal Characterization of Accelerating and Diffusing Passages Downstream of Rotating Detonation Combustors, OSTI](https://www.osti.gov/biblio/2499549)

[Feleo, Shepard, Gamba, Prediction of Detonation-Induced Disturbances Propagating Upstream into Inlets of Rotating Detonation Combustors, OSTI](https://www.osti.gov/servlets/purl/1995224)

[15-Nov-2026]

Update: no compressor anymore, so the choked injector cost gets paid by tank pressure instead. Rest holds I guess.

[15-Nov-2026]




##  Fuel type

Sixth problem is fuel and its simple, **hydrogen !!** Its a gas, mixes almost instantly and detonates easy, thats why most RDE research uses it. Jet fuel is a liquid so it has to turn into droplets and then vapor and then mix, all before the wave comes back around, soooo much harder and just more bullshit to take. Liquid hydrogen is also freezing cold so it works as the wall coolant, same trick as rockets, and it kills my cold start problem too. Catch is it takes up about 4x the space of kerosene for the same energy so it needs big round insulated tanks. Thats the planes problem though not the engines OR mine. Backup plan if hydrogen ever gets annoying is kerosene with some hydrogen mixed in 

My Sources:


[Numerical Study on Droplet Evaporation and Propagation Stability in Normal-temperature Two-phase Rotating Detonation System, arXiv](https://arxiv.org/pdf/2203.10288)

[Influence of Gaseous Hydrogen Addition on Initiation of Rotating Detonation in Liquid Fuel-Air Mixtures, Energies (MDPI)](https://www.mdpi.com/1996-1073/13/19/5101)

[15-Nov-2026]

Update: hydrogen stays, but its burning with liquid oxygen now instead of air. Tanks are my problem after all. 

[15-Nov-2026]


##  Dimensions

Seventh problem is shape and size and this is where it gets real numberful (if thats even a real word). The following is a nightmare but thats the consequences of engineering. and everything here is a first guess so its marked **to verify**. Ring size comes from how much air the engine swallows, so start there. My own cycle script (turbojet at Mach 0.8, 11 km, hydrogen, 20:1 pressure ratio, 1400 K) says 0.716 kN of thrust per 1 kg/s of air, so 15 kN needs about 21 kg/s of air and roughly 190 g/s of hydrogen. The compressor makes about 676 kPa at the ring entrance. The holes are **choked** so they pass around 1090 kg/s per m^2 of hole, and if half the ring face is holes thats about 540 kg/s per m^2 over the whole ring. Lab RDEs run 50 to 500 so we're in range. Area needed is 21 ÷ 540 = about 0.038 m^2. With a 2 cm gap the ring goes round 0.038 ÷ 0.02 = 1.9 m, so about 0.6 m across. A thin gap makes a HUGE hoop, with 8 mm it would be 1.5 m, so wide gap it is for now. The wave also needs room, a thesis gives rules of thumb. Cell size (the natural grain of the detonation) is about 9.35 mm at normal pressure and shrinks with pressure, so at roughly 3 bar (my guess) its about 3 mm. The wave needs about 12 cells of length so about 36 mm, the gap should be about 0.2 of that and at least 2.5 cells so 8 mm minimum, my 20 mm is well above that but I dont know yet if a gap that wide still holds one clean wave. Ring length has no hard rule so I picked 2 to 3 times the 36 mm, about 7 to 11 cm. Final ring is about 0.6 m across, 2 cm gap, 7 to 11 cm long, several waves. And wow fuck me I'll look like a Waterloo student after typing all of this fuck me.

*I am always open with my AI usage and the mathematics here was heavy lifted by Claude as I am no mathematician*

My Sources:

[Connolly-Boutin, Detonation Physics-Based Modelling and Design of a Rotating Detonation Engine, thesis](https://core.ac.uk/download/335015288.pdf)

[Operability of a Natural Gas-Air Rotating Detonation Engine, OSTI](https://www.osti.gov/servlets/purl/1774971)

[DLR manuscript on annulus mass flux and equivalence ratio effects in a rotating detonation combustor (title not shown, check it)](https://elib.dlr.de/139570/1/Manuskript.pdf)

[Investigating Instabilities in a Rotating Detonation Combustor, ASME Turbo Expo 2019, OSTI](https://www.osti.gov/servlets/purl/1766550)

[15-Nov-2026]

Update: all of this is the old turbojet route (air flow, compressor, Mach 0.8). SO it's all just dead numbers, redoing it for the rocket. The cell size and gap rules should still apply. 

[15-Nov-2026]

# The Rocket Route (which should've been so from the start)
 
##  Thrust, feed and pressure to consideration
 
No compressor anymore so the basics had to be picked again. Thrust first cus it decides how much propellant flows and that decides everything after it. I went with the same size as the aerospike LEAP 71 fired so theres a real engine to hold mine against which makes this much easier on me. Theirs is kerosene, mine is hydrogen powered (typical for many), the thrust number doesnt really care. Then something has to push the propellant into the ring. Pumps mean light tanks but its a turbine and compressor all over again, so **pressure-fed** it is. Thick heavy tanks but basically no moving parts which if you're a engineer or someone with more than 5 brain cells that means less points of failure. 
 
```
thrust          5 kN
feed            pressure fed (tanks pumped up, no pump since I already weighed the pros and cons)
ring pressure   15 bar = about 218 psi
```
 
218 psi sounded INSANE to me considering I've only ever dealt or worked with things that are not to that extent. So I weighed it to other things for relativity. Road bike tyre is 100 to 120 psi so its on the gentle end for a rocket. More pressure makes the ring smaller and the thrust bigger, but pressure fed means the tanks gotta hold even more than the ring does, so medium it is. Loosely locked if that's even a way to put it, might move.
 
My Sources:
 
[New aerospike engine for space travel successfully tested (LEAP 71), 3Printr](https://www.3printr.com/new-aerospike-engine-for-space-travel-successfully-tested-2676201/)
 
[15-Nov-2026]
 
 
 
 
##  Mix ratio
 
How much oxygen goes in per kilo of hydrogen. Perfect burn is 8 to 1, everything gets used up and only steam is left. My gut said slightly rich so like 6 to 7.2. Rich was right but my numbers were NOT. Extra hydrogen is super light so the exhaust shoots out faster and the flame runs cooler, same as running a car rich. BUT. Yes but hydrogen is bulky as fuck so the tanks grow, and the detonation likes it closer to 8.
 
```
O2 per kg H2    exhaust speed    tank used    cooling margin    grain size
4               3248 m/s         5.90 L/s     1.52              0.96 mm
5               3193 m/s         5.25 L/s     1.21              0.65 mm
6               3105 m/s         4.85 L/s     1.01              0.54 mm
8               2891 m/s         4.41 L/s     0.76              0.51 mm
 
cooling margin = heat the hydrogen can soak / heat the walls dump into it
 
at 5 to 1:
hydrogen can soak   0.284 kg/s x 8.8 MJ/kg          = 2.50 MW
walls dump          9.6% x 0.179 kg/s x 120 MJ/kg   = 2.06 MW
margin              2.50 / 2.06                     = 1.21
 
flow for 5 kN       5000 N / (3193 m/s x 0.92)      = 1.70 kg/s
hydrogen            1.70 / 6                        = 0.284 kg/s
oxygen              1.70 - 0.284                    = 1.42 kg/s
```
 
Cooling margin is the one that decides it. Under 1 means the walls cook up which is no bueno. At 6 its 1.01 which is zero safety, and my whole 6 to 7.2 guess fails right there. 4 has the fastest exhaust but burns 22% more tank than 6 and the grain nearly doubles. So **5 to 1**, 20% spare on cooling and under 2% off the best exhaust speed. The 9.6% wall heat number is borrowed from an air breathing hydrogen RDE so a rocket is probably worse, and the grain sizes are scaled from a number thats not sourced yet. Trust the trend more than the digits ig.
 
*I am always open with my AI usage and the mathematics here was heavy lifted by Claude as I am no mathematician, mathematic table formatted by Claude*
 
My Sources:
 
[Theuerkauf (2013), Heat Exchanger Design and Testing for a 6-Inch Rotating Detonation Engine, AFIT](https://scholar.afit.edu/etd/845)
 
[15-Nov-2026]
 
 
 
 
##  Throat and ring size
 
The throat is the pinch at the back, same as the pinched part you'd see on most jets and its what holds the pressure in. Make it wider with the same flow and the pressure drops and all the math goes with it. So the throat is the one size that pins the 15 bar in. On mine its not a hole but its a thin slit between the outer wall and the aerospike, so the bigger the ring the thinner the slit. And the waves each want their own stretch of ring, so the ring size also decides how many of them fit.
 
```
throat passes       638 kg/s per m2 at 15 bar
throat area         1.70 / 638                      = 0.00267 m2 = 26.7 cm2
 
ring 90 mm across
gap                 2669 mm2 / (3.14 x 90 mm)       = 9.4 mm
 
grain               0.65 mm
fresh layer needed  12 x 0.65                       = 7.7 mm
wave speed          85% of 3334 m/s                 = 2834 m/s
fresh mix density   2.77 kg/m3
 
waves = flow / (density x gap x layer x wave speed)
      = 1.70 / (2.77 x 0.0094 x 0.0077 x 2834)      = 3.0
 
room per wave       283 mm around / 3               = about 95 mm
wave passes a spot  2834 / 0.095                    = about 30 000 times a second
```
 
Every wave wants aboutt 95 mm of ring to itself, so 60 mm fits 2, 90 fits 3, 120 fits 4. Anything in between sits on like 2.6 waves and would keep flipping and break to more or less. More waves also means more wall for the same hydrogen to cool. Sooo I'm going with **90 mm, 9.4 mm gap, 3 waves**. Whole engine is hand sized now, the turbojet ring was 45 cm. Rocket rings run several waves anyway and NASA even found one wave alone performs worse (like I said earlier same bullshit effect with vibration motor and overall utilization). Still guesses in here so the fresh mix sitting at half the ring pressure, and the gap being the same width as the throat with no extra pinch.
 
*I am always open with my AI usage and the mathematics here was heavy lifted by Claude as I am no mathematician, mathematic table formatted by Claude*
 
My Sources:
 
[Mode-Locked Rotating Detonation Waves: Experiments and a Model Equation, arXiv](https://arxiv.org/pdf/1908.03116)
 
[Teasley et al., Heat Transfer Measurements of NASA Liquid Kerosene/Oxygen Rotating Detonation Rocket Engine, NASA NTRS](https://ntrs.nasa.gov/api/citations/20240015029/downloads/NASA%20Calorimetry%20RP%20RDRE%20AIAA%20Teasley%20Final.pdf)
 
[Connolly-Boutin, Detonation Physics-Based Modelling and Design of a Rotating Detonation Engine, thesis](https://core.ac.uk/download/335015288.pdf)
 
[15-Nov-2026]
