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
 
Update: redid the cooling with a proper rocket heat formula and the spike included, margin at 5 to 1 comes out around 2.1 instead of 1.21. Real answer is somewhere between the two. 5 to 1 stays.

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

Update: the 3.0 waves was real math on a guessed temperature. Ring is now 120 mm with a 10 mm gap, see the next parts for why as my fucking god it's a whole rabbit hole, I love it though.

[15-Nov-2026]


##  Cooling the spike and warming the oxygen
 
The aerospike sits right in the exhaust and the throat is the hottest spot on any rocket, so it needs cooling too obviously. My first thought was hollow it out and run the oxygen through veins in it, which is what LEAP 71 does. BUUUT if that wall punctures the oxygen sprays into exhaust thats full of leftover hydrogen and burns right at the hole, hole gets bigger, more oxygen, and it feeds itself completely tearing my fucking engine apart. A hydrogen leak just blows cold hydrogen along the wall cus theres no spare oxygen for it to burn with. So therefor hydrogen cools EVERYTHING. Problem two is the oxygen then shows up at the injector as a freezing liquid and it only gets about 33 millionths* (if I have that right) of a second to mix before the next wave. So same idea as the vapor chamber in my laptop (ASUS ROG G16, totally not a flex lol just straight inspo that sparked the thought), the hydrogen carries the heat away from the walls and hands it to the oxygen in a heat exchanger away from the flame. Both arrive as gas and everything works according to math.
 
```
(90 mm ring, 60 mm long, gets redone in the sizing)
 
ring walls          27.7 MW/m2 x 339 cm2            = 0.94 MW
spike               124 cm2, thins out fast         = 0.23 MW
total into walls                                    = 1.17 MW
hydrogen can soak   0.284 kg/s up to 600 K          = 2.49 MW
margin              2.49 / 1.17                     = 2.1
 
same thing with the old 9.6% rule
walls dump                                          = 2.06 MW
margin              2.50 / 2.06                     = 1.2
 
oxygen to gas       1.42 kg/s x 0.31 MJ/kg          = 0.44 MW
```
 
So. I've got two heat estimates that disagree by double which is annoying as fuck. The first is the normal rocket formula, the second is borrowed from an air breathing lab ring. NASA measured a kerosene ring and got heat close to normal rocket theory so its probably nearer 2 than 1.2. Either way its above 1 and the hydrogen has the 0.44 MW to spare for the oxygen. The catch with the exchanger is obvious, its hydrogen and oxygen one wall apart, if that cracks they mix and everything goes to shit and falls apart dramatically. Difference is that wall sits somewhere cool and quiet so it can be thick and **double walled with a gap** in between, so a leak goes into the gap and out. In the spike it would be thin, in the hottest spot, getting hammered 30 000 times a second. The puncture and leak part is general rocket knowledge, still gotta find a proper source for it.
 
*I am always open with my AI usage and the mathematics here was heavy lifted by Claude as I am no mathematician, mathematic table formatted by Claude*
 
My Sources:
 
[New aerospike engine for space travel successfully tested (LEAP 71), 3Printr](https://www.3printr.com/new-aerospike-engine-for-space-travel-successfully-tested-2676201/)
 
[Teasley et al., Heat Transfer Measurements of NASA Liquid Kerosene/Oxygen Rotating Detonation Rocket Engine, NASA NTRS](https://ntrs.nasa.gov/api/citations/20240015029/downloads/NASA%20Calorimetry%20RP%20RDRE%20AIAA%20Teasley%20Final.pdf)
 
[15-Nov-2026]
 
 
 
 
##  Why the ring grew
 
Turns out how warm the mix is when it enters the ring decides the wave count almost by itself. Cold gas is denser and its grain (idk if I explained it already but grain is the space that the shockwave wants to use up.) is bigger so each wave eats a bigger chunk of ring and fewer fit. And I cant pin that temperature down cus it depends on the wall heat, which I have two estimates for. So my clean 3.0 waves was built on a guess which I know I know isn't amazing but hey can you blame me ?? I'm not even an engineer just a bored fucking guy.
 
```
mix temperature     waves in a 90 mm ring     ring size for 3 waves
180 K (cold)        1.5                       181 mm
260 K               2.4                       115 mm
300 K (my guess)    3.0                       91 mm
350 K               4.0                       68 mm
 
low heat estimate   mix arrives around 180 K
high heat estimate  mix arrives around 345 K
 
flow per ring area
90 mm, gap = throat     1.70 / 26.7 cm2             = 638 kg/s per m2
120 mm, 10 mm gap       3.14 x 120 x 10             = 37.7 cm2
                        1.70 / 37.7 cm2             = 451 kg/s per m2
pinch                   37.7 / 26.7                 = 1.4
```
 
So with that I went and looked at what real rocket rings look like. University of Washington ran 25, 51 and 76 mm rings all with a 5 mm gap, the Air Force one is 76 mm and takes up to 0.68 kg/s. I'm pushing 1.7 so bigger than those makes sense. Bigger rings carried more waves in their tests (which is obvious. More space for higher grain), and real waves ran 20 to 40% slower than the ideal speed where I assumed 15%. So forget exactly 3 its several and the ring decides. The actual reason to go bigger is flow per area. Those rings ran at 80 to 400 and mine was at 638 cus I made the gap the same width as the throat, thats outside anything tested. So **120 mm ring, 10 mm gap** and a mild pinch at the exit. Mild cus the Air Force tried tighter pinches and got waves running against eachother and more unsteadiness which obviously isn't satisfactory.
 
*I am always open with my AI usage and the mathematics here was heavy lifted by Claude as I am no mathematician, mathematic table formatted by Claude*
 
My Sources:
 
[Mundt, Knowlen, Kurosaka (2024), Scale effects on rotating detonation rocket engine operation](https://doaj.org/article/5eae51e875de4b09b5c54c29abaa5bad)
 
[Knowlen, Mundt, Kurosaka (2023), Experimental results for 25-mm and 51-mm rotating detonation rocket engine combustors, Shock Waves](https://doi.org/10.1007/s00193-023-01120-x)
 
[Bennewitz et al. (2021), Performance of a Rotating Detonation Rocket Engine with Various Convergent Nozzles and Chamber Lengths, Energies](https://mdpi.com/1996-1073/14/8/2037)
 
[Koch et al., Multi-scale Physics of Rotating Detonation Engines: Autosolitons and Modulational Instabilities, arXiv](https://arxiv.org/pdf/2003.06655)
 
[15-Nov-2026]
 
 
 
 
##  Hydrogen lights too easy
 
I wrote earlier that hydrogen detonates easy. Half the story. It also BURNS easy, and the burning can win. Its called pre ugnition which is same as a petrol engine where the mix lights before the spark. Hydrogen and oxygen can light the instant they touch, right at the injector as a normal flame, and then when the wave comes around the fresh layer it was supposed to eat is already burnt. Purdue ran hydrogen at rocket pressures and mostly got a flame sitting at the injector instead of detonation with eroded injectors. Their pressures were 61 to 381 psia and I'm at 218 so that's my problem too. A German lab ring did get hydrogen and oxygen to detonate, 3 to 5 waves at 25 to 38 kHz in a 68 mm ring, but the waves only ran at about 0.53 to 0.65 of the ideal speed. The fixes are the same as a car which also brought up the following ideas. Higher octane (methane equivelent for jets), dont lug it (push the mix through fast) and kill the hot spots (injector with no dead corners).
 
```
5 kN, 15 bar            hydrogen (5 to 1)     methane (3 to 1)
exhaust speed           3193 m/s              2513 m/s
propellant flow         1.70 kg/s             2.16 kg/s
tank used               5.25 L/s              2.70 L/s
fuel can soak           2.49 MW               0.91 MW
cooling margin          2.1                   0.8
```
 
Methane is a easy fuel and its what most of the rings that ran well used. Half the tank too. But the exhaust is slower and it cant cool the engine by itself, margin is under 1, so it would need extra tricks which means more moving parts which means more points of failure. Hydrogens one real problem is the injector and thats a design job I can go at directly. NASA ran a ring on liquid oxygen with hydrogen gas and the hardware survived so thankfully its not a dead end. Meaning its LOCKED IN that I'm staying on **hydrogen**, plus my whole research is built on it. The German ring ran at 30 to 50 kg/s per m2 and wanted more and I'm at about 450 so I'm already not lugging it.
 
*I am always open with my AI usage and the mathematics here was heavy lifted by Claude as I am no mathematician, mathematic table formatted by Claude*
 
My Sources:
 
[Stechmann (2017), Experimental Study of High-Pressure Rotating Detonation Combustion in Rocket Environments, Purdue](https://docs.lib.purdue.edu/dissertations/AAI10684279)
 
[Armbruster et al. (2023), Experimental Investigation of a Small-Scale Oxygen-Hydrogen Rotating Detonation Combustor, DLR](https://elib.dlr.de/198217/1/ISTS%20Exp%20Investig%202023-a-2-05.pdf)
 
[Teasley, Fedotowsky, Gradl, Current State of NASA Continuously Rotating Detonation Cycle Engine Development, NASA NTRS](https://ntrs.nasa.gov/api/citations/20220018157/downloads/Current%20State%20of%20NASA%20Continuous%20Detonation%20Cycle%20Engine%20Development%20AIAA%20Teasley%20paper.pdf)
 
[15-Nov-2026]
 
 
 
 
##  Injector
 
This is the part that decides if hydrogen works at all which both rings I read about use the same layout, pairs of holes with the two jets aimed at eachother, one hydrogen one oxygen. Two garden hoses pointed so the streams crash together for a great violent mix. They stay in separate pipes the whole way and only meet where they collide, inside the ring and never premixed or carburated whatever the term is. I want them to mash in the middle of the gap and not against the metal so if a flame does sit somewhere its sitting in gas. Too close to the face and the flame parks on the metal, too far out and the bottom of the ring holds gas that isnt mixed yet. So a few mm off the face. And lots of small pairs over a few big ones for an even coat cus patchy layer means patchy wave.
 
```
feed pressure       30 bar (twice the ring)
 
hole area needed    hydrogen 168 mm2      oxygen 197 mm2
 
pairs     hydrogen hole     oxygen hole     spacing
36        2.4 mm            2.6 mm          10.5 mm
72        1.7 mm            1.9 mm          5.2 mm
120       1.3 mm            1.5 mm          3.1 mm
240       0.9 mm            1.0 mm          1.6 mm
 
120 pairs
hydrogen  168 / 120 = 1.40 mm2 each       = 1.3 mm hole
oxygen    197 / 120 = 1.64 mm2 each       = 1.5 mm hole
spacing   377 mm around / 120             = 3.1 mm
```
 
Going too small has its own bullshit. Tiny holes clog,tiny jets run out of push before they reach the middle and the holes need metal between them. So **120 pairs**, holes come out almost the same size as the German ring (1.0 and 1.5 mm) which has been built and fired and theres still about 1.7 mm of metal between holes. Not gonna call it the best though cus the German ring had slow waves and they wanted to redo their injector, nobody has a proven best for this yet. Hole sizes assume both arrive as cold gas around 200 to 230 K and that only 80% of each hole actually flows.
 
*I am always open with my AI usage and the mathematics here was heavy lifted by Claude as I am no mathematician, mathematic table formatted by Claude*
 
My Sources:
 
[Armbruster et al. (2023), Experimental Investigation of a Small-Scale Oxygen-Hydrogen Rotating Detonation Combustor, DLR](https://elib.dlr.de/198217/1/ISTS%20Exp%20Investig%202023-a-2-05.pdf)
 
[Bennewitz et al. (2021), Performance of a Rotating Detonation Rocket Engine with Various Convergent Nozzles and Chamber Lengths, Energies](https://mdpi.com/1996-1073/14/8/2037)
 
[15-Nov-2026]




 ##  Does it all work together
 
Picking every part one by one is nice but they all push on eachother, so everything went into one script that sizes the whole rocket and checks each pick against the rest. Ran it twice cus I still have two heat estimates and cant narrow it. Nothing fails. 6 things to keep an eye on though fuck.
 
```
5 kN · hydrogen + oxygen 5 to 1 · 1.70 kg/s · ring 15 bar · feed 30 bar
ring 120 mm · gap 10 mm · 50 mm long · 120 jet pairs
 
throat area         26.7 cm2
ring face           3.14 x 120 x 10                 = 37.7 cm2
pinch               37.7 / 26.7                     = 1.41
flow per ring area  1.70 / 37.7 cm2                 = 452 kg/s per m2
 
                            low heat        high heat
heat into walls             1.59 MW         2.07 MW
hydrogen can soak           2.49 MW         2.49 MW
cooling margin              1.56            1.20
hydrogen leaves walls at    381 K           about 500 K
hydrogen at the injector    275 K           391 K
oxygen at the injector      200 K           200 K
waves                       2.6             4.4
wave rate                   19 kHz          25 kHz
fresh layer                 8.5 mm          about 7 mm
jets meet                   2.6 mm off the face (both)
 
aerospike           114 mm long · exhaust leaves at Mach 2.38
whole engine        240 mm long · 156 mm across (390 mm with the exchanger)
tanks               hydrogen about 37 bar · oxygen about 32 bar · drain 5.25 L/s
 
hot hydrogen is thinner so the same hole passes less of it
holes sized for 275 K, hydrogen arrives at 391 K    mix drifts 5 to about 6
holes sized for 391 K, hydrogen arrives at 275 K    mix drifts 5 to about 4.2
```
 
What passes in both cases is thrust, the pinch (Air Force tested 1.23, 1.62 and 2.40 so 1.41 is on the mild side), flow per area, the exchanger pushing heat the right way with both arriving as gas, and the gap, length and diameter all being way above what the wave needs. The jets hit eachother with nearly equal push so the mix goes straight down the ring. What changed is the pinch costs heat. The narrowing part between the ring and the throat adds 0.58 MW I hadnt counted, so the margin is 1.56 at best and 1.20 at worst instead of the 2.1 from before.
 
The one that only showed up cus everything was in one place is the mix drifting with temperature. Two ways to fix it. A control valve, which is basically fuel injection with an ECU or fixed holes sized for the worst case, which is a carb with fixed jets. Went with fixed holes sized for hot hydrogen. No moving parts and when its wrong it runs rich, cooler flame and more coolant, so it fails toward safe. Sized the other way it fails lean and thats where the walls cook. Also had to pick a route for the hydrogen. In at the nozzle end, forward through the outer wall, across the injector plate, back down the inner wall and the spike, up a tube on the axis into the exchanger and then to the manifold. One long path so nothing is left uncooled, the 5 bar it loses on the way is a guess.
 
Still watching: wave count is 2.6 to 4.4 so several but never a clean number. The pressure right behind a wave peaks around 172 bar against a 30 bar feed so the jets get blocked every single pass, sadly thats just how these work. Pre ignition is NOT in the math, the cold mix wont light by itself between waves but hot burnt gas touching it is the real risk. Wall thickness is somewhere between 0.7 mm (average pressure) and 7.5 mm (if the peak hit everywhere at once, which it doesnt). And nothing here has been stress checked.
 
*I am always open with my AI usage and the mathematics here was heavy lifted by Claude as I am no mathematician, mathematic table formatted by Claude*
 
My Sources:
 
[Bennewitz et al. (2021), Performance of a Rotating Detonation Rocket Engine with Various Convergent Nozzles and Chamber Lengths, Energies](https://mdpi.com/1996-1073/14/8/2037)
 
[Knowlen, Mundt, Kurosaka (2023), Experimental results for 25-mm and 51-mm rotating detonation rocket engine combustors, Shock Waves](https://doi.org/10.1007/s00193-023-01120-x)
 
[15-Nov-2026]
