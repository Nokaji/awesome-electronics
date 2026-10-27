# Awesome Electronics

> A curated list of resources to learn, design, build, measure and repair electronics, from your first LED to designing open source silicon chips.

This list covers electronics **in the broad sense**: analog, digital, microcontrollers, FPGAs, PCB design, simulation, test and measurement, power, RF, audio, hardware security, open source silicon, sourcing, manufacturing and communities.

**Legend**: **bold name** = essential resource · (FR) = French-language resource · (free) = free or open source · (paid) = paid · (freemium) = free tier plus paid plans

**Inspirations and sources**: [kitspace/awesome-electronics](https://github.com/kitspace/awesome-electronics) (the main English-language reference), [techgaun/awesome-electronics](https://github.com/techgaun/awesome-electronics), [hdl/awesome](https://github.com/hdl/awesome) (HDL and verification). This list follows their spirit and adds a French-language layer, the 2026 landscape (end of EAGLE, open source silicon) and learning paths.

> **Reliability note**: several facts in this list were rechecked in October 2026 (end of EAGLE, state of Tiny Tapeout, ChipFoundry, wafer.space, popularity of the reference lists). The other links come from established resources but were not all opened one by one. When a deep path changes often, the link points to the site root. If a link is broken, open an issue or a pull request.

---

## Table of Contents

- [Learning Paths](#learning-paths)
- [Learn](#learn)
  - [Courses and MOOCs](#courses-and-moocs)
  - [Tutorials and Educational Sites](#tutorials-and-educational-sites)
  - [Books](#books)
  - [Mathematics and Signal Theory](#mathematics-and-signal-theory)
  - [Starter Kits and Platforms](#starter-kits-and-platforms)
- [Simulation](#simulation)
- [Calculators and Design Tools](#calculators-and-design-tools)
- [Schematic and PCB Design (EDA)](#schematic-and-pcb-design-eda)
  - [EDA Software](#eda-software)
  - [KiCad Ecosystem](#kicad-ecosystem)
  - [Component Libraries and 3D Models](#component-libraries-and-3d-models)
  - [Layout, EMC and Signal Integrity Best Practices](#layout-emc-and-signal-integrity-best-practices)
  - [PCB Fabrication and Assembly](#pcb-fabrication-and-assembly)
  - [Hardware as Code and CI](#hardware-as-code-and-ci)
- [Components and Sourcing](#components-and-sourcing)
- [Analog Electronics](#analog-electronics)
- [Digital Electronics, Logic and FPGA](#digital-electronics-logic-and-fpga)
- [Microcontrollers and Embedded Systems](#microcontrollers-and-embedded-systems)
- [Power Electronics, Power Supplies and Batteries](#power-electronics-power-supplies-and-batteries)
- [RF, Antennas, SDR and Signal Processing](#rf-antennas-sdr-and-signal-processing)
- [Audio, Synthesizers and Instruments](#audio-synthesizers-and-instruments)
- [Test and Measurement Equipment](#test-and-measurement-equipment)
- [Soldering, Assembly and Mechanics](#soldering-assembly-and-mechanics)
- [Troubleshooting, Repair and Reverse Engineering](#troubleshooting-repair-and-reverse-engineering)
- [Hardware Security](#hardware-security)
- [Open Source Silicon (Chip Design)](#open-source-silicon-chip-design)
- [Home Automation, IoT and Robotics](#home-automation-iot-and-robotics)
- [Standards, Compliance and Regulation](#standards-compliance-and-regulation)
- [Open Source Hardware](#open-source-hardware)
- [Videos, Podcasts, Blogs and Magazines](#videos-podcasts-blogs-and-magazines)
- [Communities and Forums](#communities-and-forums)
- [French-Language Resources](#french-language-resources)
- [Other Awesome Lists](#other-awesome-lists)
- [Contributing](#contributing)
- [License](#license)

---

## Learning Paths

Three trajectories so you do not get lost. Each step points to the detailed sections below.

### 1. Complete beginner (0 to 3 months)

1. Understand voltage, current, resistance, Ohm's law and voltage dividers: [Khan Academy](https://www.khanacademy.org/science/electrical-engineering), [All About Circuits (textbook)](https://www.allaboutcircuits.com/textbook/).
2. Experiment in the browser, risk-free: [Falstad](https://www.falstad.com/circuit/), [Tinkercad Circuits](https://www.tinkercad.com/circuits), [Wokwi](https://wokwi.com/).
3. Buy a decent multimeter, a breadboard, a current-limited power supply and a temperature-controlled soldering iron ([Test and Measurement](#test-and-measurement-equipment), [Soldering](#soldering-assembly-and-mechanics)).
4. First book: *Make: Electronics* (Charles Platt). Do all the experiments.
5. First microcontroller: Arduino or Raspberry Pi Pico ([Embedded](#microcontrollers-and-embedded-systems)).

### 2. Intermediate (3 to 12 months)

1. Solid theory: [MIT 6.002](https://ocw.mit.edu/courses/6-002-circuits-and-electronics-spring-2007/), *Practical Electronics for Inventors*.
2. Serious simulation: [LTspice](https://www.analog.com/en/resources/design-tools-and-calculators/ltspice-simulator.html) or [ngspice](https://ngspice.sourceforge.io/).
3. First PCB in [KiCad](https://www.kicad.org/), made by a prototyping house ([Fabrication](#pcb-fabrication-and-assembly)).
4. Switching supplies, op-amps, ADCs: [TI Precision Labs](https://www.ti.com/), [Analog Devices](https://www.analog.com/en/education/education-library.html).
5. Instruments: oscilloscope, logic analyzer ([sigrok](https://sigrok.org/)).

### 3. Advanced (1 year and beyond)

1. *The Art of Electronics* (3rd ed.) and *High-Speed Digital Design*.
2. Signal integrity, EMC, layout ([dedicated section](#layout-emc-and-signal-integrity-best-practices)).
3. Open source FPGAs ([Project F](https://projectf.io/), [Yosys](https://github.com/YosysHQ/yosys)) or RF ([Microwaves101](https://www.microwaves101.com/)).
4. CE and EMC compliance ([Standards](#standards-compliance-and-regulation)).
5. Chip design: [Tiny Tapeout](https://tinytapeout.com/), [Zero to ASIC](https://zerotoasiccourse.com/).

---

## Learn

### Courses and MOOCs

- **[MIT OpenCourseWare: 6.002 Circuits and Electronics](https://ocw.mit.edu/courses/6-002-circuits-and-electronics-spring-2007/)** (free) - The reference course on linear circuits, MOSFETs, digital abstraction and amplifiers (companion book: *Foundations of Analog and Digital Electronic Circuits*).
- [MIT OpenCourseWare](https://ocw.mit.edu/) (free) - Full catalog: signals and systems (6.003), electromagnetics, microelectronics, embedded systems.
- [edX](https://www.edx.org/learn/circuits) / [Coursera](https://www.coursera.org/) (free to audit) - Circuits and electronics courses from major universities.
- [NPTEL](https://nptel.ac.in/) (free) - Indian university (IIT) video courses: analog and digital electronics, power electronics, VLSI.
- [Khan Academy: Electrical Engineering](https://www.khanacademy.org/science/electrical-engineering) (free) - Very good entry point to basic circuits.
- [FUN MOOC](https://www.fun-mooc.fr/) (FR) (free) - French university MOOC platform, with electronics and embedded systems courses depending on the session.
- [Digilent Reference: Real Analog course](https://digilent.com/reference/) (free) - Circuits course designed to be followed with Analog Discovery hardware.
- [Analog Devices: Education Library](https://www.analog.com/en/education/education-library.html) (free) - Educational tutorials, videos and application notes (see also the university program around the ADALM2000).
- [TI Precision Labs](https://www.ti.com/) (free) - Texas Instruments video series and exercises on op-amps, ADCs, sensors and power supplies (search for "Precision Labs").
- [Nand2Tetris](https://www.nand2tetris.org/) (free) - Build a complete computer, from NAND gates up to software.
- [Ben Eater: 8-bit computer](https://eater.net/) (free) - Building an 8-bit processor on breadboards, the best visual introduction to how a CPU works.
- [Contextual Electronics](https://contextualelectronics.com/) (paid) - Structured PCB and product design courses (Chris Gammell).
- [FEDEVEL Academy](https://fedevel.education/) (paid) - PCB design training (Robert Feranec) with complete projects.
- [Udemy: Electronics](https://www.udemy.com/topic/electronics/) (paid) - Quality varies widely; read the reviews before buying.

### Tutorials and Educational Sites

- **[All About Circuits: Textbook](https://www.allaboutcircuits.com/textbook/)** (free) - Online textbook covering DC, AC, semiconductors, digital and logic.
- [Lessons In Electric Circuits (Tony Kuphaldt)](https://www.ibiblio.org/kuphaldt/electricCircuits/) (free) - The original open textbook, in several volumes.
- [Electronics Tutorials](https://www.electronics-tutorials.ws/) (free) - Illustrated tutorials for beginners and intermediate learners.
- [Electronics Notes](https://www.electronics-notes.com/) (free) - Reference notes on components, RF, communications and measurement.
- [The Electronics Club](https://electronicsclub.info/) (free) - Simple tutorials for teaching and beginners.
- [SparkFun Learn](https://learn.sparkfun.com/) (free) - Hands-on guides: multimeters, soldering, protocols (I2C, SPI, UART), sensors.
- [Adafruit Learn](https://learn.adafruit.com/) (free) - Thousands of project and component guides.
- [Circuit Digest](https://circuitdigest.com/) (free) - Circuit projects and tutorials.
- [Electronics Stack Exchange](https://electronics.stackexchange.com/) (free) - When you have a precise question, the answer often already exists there.
- [Analog Devices: Analog Dialogue](https://www.analog.com/en/resources/analog-dialogue.html) (free) - In-depth technical articles on analog and mixed-signal design.
- [EDN Design Ideas](https://www.edn.com/) (free) - Clever circuits submitted by engineers.
- [Instructables](https://www.instructables.com/) / [Hackster.io](https://www.hackster.io/) / [Hackaday.io](https://hackaday.io/) (free) - Step-by-step documented projects.
- [Soldering Is Easy](https://mightyohm.com/blog/2011/04/soldering-is-easy-comic-book-downloads/) (free) - A soldering mini comic book.
- [Zeste de Savoir](https://zestedesavoir.com/) (FR) (free) - French-language tutorials (including electronics and Arduino) written by the community.
- [Eskimon](https://eskimon.fr/) (FR) (free) - French-language tutorials for getting started with Arduino.
- [Locoduino](https://www.locoduino.org/) (FR) (free) - French-language community and articles around Arduino (originally for model railways).
- [ABC Electronique](https://www.abcelectronique.com/) (FR) (free) - Courses, schematics and projects in French.

### Books

**General and reference**

- ***The Art of Electronics* (3rd ed.)** - Paul Horowitz, Winfield Hill. The electronics engineer's bible. French edition: *Traité de l'électronique analogique et numérique* (Elektor, earlier edition).
- ***Learning the Art of Electronics*** - Thomas Hayes, Paul Horowitz. The companion hands-on course, designed to be done in the lab.
- *The Art of Electronics: The x-Chapters* - Additional chapters (transistors, power, instrumentation and more).
- *Practical Electronics for Inventors* - Paul Scherz, Simon Monk. Excellent general reference.
- *Make: Electronics* - Charles Platt. Learning by experiment.
- *Make: More Electronics* - Charles Platt. Sequel: logic, amplifiers, sensors.
- *Encyclopedia of Electronic Components* (Vol. 1 to 3) - Charles Platt. How components work and how to use them.
- *Getting Started in Electronics* - Forrest Mims. A classic in handwritten notebook style.
- *Foundations of Analog and Digital Electronic Circuits* - Anant Agarwal, Jeffrey Lang. Textbook of MIT course 6.002.
- *Open Circuits* - Windell Oskay, Eric Schlaepfer. Gorgeous photographs and cross-sections of components.

**Analog**

- *Microelectronic Circuits* - Sedra, Smith. The standard university textbook.
- *Fundamentals of Microelectronics* - Behzad Razavi.
- *Analysis and Design of Analog Integrated Circuits* - Gray, Hurst, Lewis, Meyer.
- *Design of Analog CMOS Integrated Circuits* - Behzad Razavi.
- [Op Amps For Everyone](https://www.ti.com/lit/an/slod006b/slod006b.pdf) (free) - Ron Mancini (Texas Instruments).
- *Analog Circuit Design* (3 volumes) - Jim Williams and contributors. Anecdotes and circuits from the Linear Technology school.
- *Troubleshooting Analog Circuits* - Bob Pease.
- *The Data Conversion Handbook* - Analog Devices.

**Digital, FPGA, architecture**

- *Digital Design and Computer Architecture* - Sarah Harris, David Harris.
- *Computer Organization and Design* - Patterson, Hennessy.
- *Digital Design: Principles and Practices* - John Wakerly.
- *FPGA Prototyping by Verilog Examples* - Pong P. Chu.

**Embedded**

- *Making Embedded Systems* - Elecia White.
- *The Definitive Guide to ARM Cortex-M3 and Cortex-M4 Processors* - Joseph Yiu.
- *Designing Embedded Hardware* - John Catsoulis.
- [The Embedded Rust Book](https://docs.rust-embedded.org/book/) (free) - Rust on microcontrollers.

**PCB, EMC, signal integrity**

- ***High-Speed Digital Design: A Handbook of Black Magic*** - Howard Johnson, Martin Graham.
- *Signal and Power Integrity - Simplified* - Eric Bogatin.
- *Electromagnetic Compatibility Engineering* - Henry W. Ott.
- *Printed Circuit Board Design Techniques for EMC Compliance* - Mark Montrose.
- *PCB Design for Real-World EMI Control* - Bruce Archambeault.
- *Right the First Time* - Lee Ritchey. High-speed PCB practice.

**Power**

- *Fundamentals of Power Electronics* - Robert Erickson, Dragan Maksimovic.
- *Power Electronics: Converters, Applications, and Design* - Mohan, Undeland, Robbins.
- *Switching Power Supplies A to Z* - Sanjaya Maniktala.
- *Switching Power Supply Design* - Abraham Pressman.

**RF and radio**

- *RF Circuit Design* - Chris Bowick.
- *RF Microelectronics* - Behzad Razavi.
- *Microwave Engineering* - David Pozar.
- *The ARRL Handbook* - The radio amateur's reference.
- *Experimental Methods in RF Design* - ARRL.

**Audio**

- *Audio Power Amplifier Design* - Douglas Self.
- *Small Signal Audio Design* - Douglas Self.

**Hardware security**

- *The Hardware Hacking Handbook* - Jasper van Woudenberg, Colin O'Flynn.
- *Hacking the Xbox* (free online) - Andrew "bunnie" Huang.

### Mathematics and Signal Theory

- [Paul's Online Math Notes](https://tutorial.math.lamar.edu/) (free) - Calculus, differential equations, Laplace transforms.
- [3Blue1Brown](https://www.3blue1brown.com/) (free) - Visual intuition (linear algebra, Fourier transform).
- [The Scientist and Engineer's Guide to DSP](http://www.dspguide.com/) (free) - Steven W. Smith's complete book on signal processing.
- [DSPRelated](https://www.dsprelated.com/) (free) - DSP articles and forum.
- [Think DSP](https://greenteapress.com/wp/think-dsp/) (free) - DSP with Python.
- [The Feynman Lectures on Physics, Vol. II](https://www.feynmanlectures.caltech.edu/) (free) - Electromagnetism.
- [MIT OCW 6.003 Signals and Systems](https://ocw.mit.edu/) (free) - Mathematical foundations of system analysis.
- [Control Systems Lectures (Brian Douglas)](https://engineeringmedia.com/) (free) - Control theory explained visually.

### Starter Kits and Platforms

- [Arduino Starter Kit](https://www.arduino.cc/) - The classic way to start.
- [Raspberry Pi Pico](https://www.raspberrypi.com/documentation/microcontrollers/) - RP2040/RP2350 microcontroller with excellent documentation.
- [SparkFun Inventor's Kit](https://www.sparkfun.com/) - Guided kit.
- [Kitronik](https://kitronik.co.uk/) - Educational kits.
- [Snap Circuits](https://www.elenco.com/) - For younger learners, no soldering.
- [Digilent Analog Discovery](https://digilent.com/) - Portable USB lab (scope, generator, power supply, logic analyzer).
- [Analog Devices ADALM2000](https://www.analog.com/en/resources/evaluation-hardware-and-software/evaluation-boards-kits/adalm2000.html) - Portable USB learning lab.
- [Kubii](https://www.kubii.com/) (FR) - Raspberry Pi and accessories, in France.

---

## Simulation

**SPICE and circuit simulators**

- **[LTspice](https://www.analog.com/en/resources/design-tools-and-calculators/ltspice-simulator.html)** (free) - Analog Devices' SPICE simulator, widely used for power and analog design. Windows and macOS.
- [ngspice](https://ngspice.sourceforge.io/) (free) - Open source SPICE simulator, integrated in KiCad.
- [Xyce](https://xyce.sandia.gov/) (free) - Sandia National Labs' parallel simulator, for very large circuits.
- [Qucs-S](https://github.com/ra3xdh/qucs_s) (free) - Graphical front end for ngspice/Xyce, useful for RF.
- [QSPICE](https://www.qorvo.com/design-hub/design-tools/interactive/qspice) (free) - Qorvo's simulator (Mike Engelhardt), very fast for power electronics.
- [PSpice (Cadence)](https://www.orcad.com/) (free tier) - Student / lite version available.
- [TINA-TI](https://www.ti.com/tool/TINA-TI) (free) - Texas Instruments' SPICE with TI component models.
- [SIMetrix](https://www.simetrix.co.uk/) (paid) - Professional SPICE simulator.
- [Proteus](https://www.labcenter.com/) (paid) - Simulation with microcontroller co-simulation.
- [NI Multisim](https://www.ni.com/) (paid) - Simulation for education.
- [GeckoCIRCUITS](https://github.com/geckocircuits/GeckoCIRCUITS) (free) - Power electronics simulation.
- [PLECS](https://www.plexim.com/) (paid) - Power systems simulation.

**Online and interactive simulation**

- **[Falstad Circuit Simulator](https://www.falstad.com/circuit/)** (free) - Real-time visual simulation, ideal for building intuition.
- [Wokwi](https://wokwi.com/) (free) - Online simulation of Arduino, ESP32 and Pico.
- [Tinkercad Circuits](https://www.tinkercad.com/circuits) (free) - Simple simulation, well suited to teaching.
- [CircuitLab](https://www.circuitlab.com/) (freemium) - Browser-based editor and simulator.
- [EveryCircuit](https://everycircuit.com/) (freemium) - Animated simulation (web and mobile).
- [CircuitVerse](https://circuitverse.org/) (free) - Digital logic simulation.
- [Digital](https://github.com/hneemann/Digital) (free) - Digital logic simulator for teaching.

**Electromagnetics and thermal**

- [openEMS](https://openems.de/) (free) - Open source FDTD solver for antennas and transmission lines.
- [FEMM](https://www.femm.info/) (free) - 2D finite element analysis for magnetics (inductors, transformers, motors).
- [Elmer FEM](https://www.elmerfem.org/) (free) - Multiphysics finite element solver.
- [4nec2](https://www.qsl.net/4nec2/) / [xnec2c](https://github.com/KJ7LNW/xnec2c) (free) - Antenna modeling (NEC).
- [scikit-rf](https://scikit-rf.org/) (free) - RF network analysis in Python (S-parameters, Smith chart).

**Python for electronics**

- [PySpice](https://github.com/PySpice-org/PySpice) (free) - Drive ngspice from Python.
- [Schemdraw](https://schemdraw.readthedocs.io/) (free) - Draw schematics with code.
- [Lcapy](https://lcapy.readthedocs.io/) (free) - Symbolic analysis of linear circuits.
- [SKiDL](https://github.com/devbisme/skidl) (free) - Describe circuits in Python.
- [PyVISA](https://pyvisa.readthedocs.io/) (free) - Control test instruments.
- [SymPy](https://www.sympy.org/) (free) - Symbolic math for deriving transfer functions.

---

## Calculators and Design Tools

- **[Saturn PCB Toolkit](https://saturnpcb.com/saturn-pcb-toolkit/)** (free) - Trace width, impedance, current, vias, spacing.
- [KiCad Calculator Tools](https://www.kicad.org/) (free) - Built-in calculators (trace, impedance, color code, regulator).
- [Digi-Key Calculators](https://www.digikey.com/en/resources/conversion-calculators) (free) - Common conversions and calculations.
- [TI WEBENCH](https://webench.ti.com/) (free) - Design of power supplies and filters with TI parts.
- [Analog Devices Design Tools](https://www.analog.com/en/design-center/design-tools-and-calculators.html) (free) - LTpowerCAD, filters, ADC calculations and more.
- [Wurth REDEXPERT](https://www.we-online.com/en/components/redexpert) (free) - Inductor and capacitor selection and loss simulation.
- [Coilcraft Tools](https://www.coilcraft.com/) (free) - Inductor selection tools.
- [Infineon Design Tools](https://www.infineon.com/) (free) - Sizing tools for power semiconductors.
- [Octopart](https://octopart.com/) (free) - Parametric search and pricing.

---

## Schematic and PCB Design (EDA)

### EDA Software

> **Important change**: Autodesk ended sales and support of EAGLE on June 7, 2026. The path Autodesk proposes is Fusion Electronics; KiCad can import EAGLE files.

**Open source**

- **[KiCad](https://www.kicad.org/)** (free) - Complete open source EDA suite: schematic, PCB, 3D viewer, ngspice simulation, Python scripting. The de facto standard in open source hardware.
- [LibrePCB](https://librepcb.org/) (free) - Simpler than KiCad, with cleanly managed libraries.
- [Horizon EDA](https://horizon-eda.org/) (free) - Design centered on part and pool management.
- [gEDA / PCB](http://www.geda-project.org/) (free) - Historical suite (little new development).
- [Fritzing](https://fritzing.org/) (free) - Prototyping and breadboard-view oriented, useful for teaching.

**Cloud and freemium**

- [EasyEDA](https://easyeda.com/) (freemium) - Online EDA tied to LCSC and JLCPCB, very handy for assembly.
- [Flux](https://www.flux.ai/) (freemium) - Collaborative browser-based EDA with AI assistants.
- [CircuitMaker](https://circuitmaker.com/) (free) - Altium's community edition (public projects).
- [Autodesk Fusion (Electronics)](https://www.autodesk.com/products/fusion-360/) (paid) - Replaces EAGLE; integrated mechanical and electronic design.

**Professional**

- [Altium Designer](https://www.altium.com/) (paid) - The PCB reference in industry.
- [Cadence OrCAD / Allegro](https://www.orcad.com/) (paid) - Complete toolchain for complex PCBs.
- [Siemens Xpedition / PADS](https://eda.sw.siemens.com/) (paid) - High-density board design.
- [Zuken CR-8000](https://www.zuken.com/) (paid) - Board and system design.
- [DipTrace](https://diptrace.com/) (paid) - Affordable alternative.

### KiCad Ecosystem

- [KiCad Plugin and Content Manager](https://www.kicad.org/) (free) - Install extensions, libraries and themes from the application.
- [KiBot](https://github.com/INTI-CMNB/KiBot) (free) - Automate generation of Gerbers, BOMs, PDFs and renders (CI).
- [KiKit](https://github.com/yaqwsx/KiKit) (free) - Panelization and manufacturing automation.
- [InteractiveHtmlBom](https://github.com/openscopeproject/InteractiveHtmlBom) (free) - Interactive BOM for manual assembly.
- [Freerouting](https://github.com/freerouting/freerouting) (free) - Open source autorouter.
- [KiCad Libraries (official)](https://gitlab.com/kicad/libraries) (free) - Symbols, footprints, 3D models.
- [Kitspace](https://kitspace.org/) (free) - Hosting and sharing of PCB projects, one-click BOM purchasing.
- [KiCad Forum](https://forum.kicad.info/) (free) - Official, very active forum.
- [kicad-jlcpcb-tools](https://github.com/Bouni/kicad-jlcpcb-tools) (free) - Link your BOM to JLCPCB assembly part numbers.

### Component Libraries and 3D Models

- [SnapMagic (formerly SnapEDA)](https://www.snapeda.com/) (free) - Symbols, footprints and 3D models for many tools.
- [Ultra Librarian](https://www.ultralibrarian.com/) (free) - Manufacturer CAD libraries.
- [Component Search Engine](https://componentsearchengine.com/) (free) - CAD models for common components.
- [LCSC / EasyEDA library](https://www.lcsc.com/) (free) - Very large library, tied to LCSC stock.
- [Digi-Key / Mouser / Farnell](#distributors) - Also provide per-part CAD models.

> Always check a downloaded footprint against the component datasheet before ordering boards.

### Layout, EMC and Signal Integrity Best Practices

- **[Rick Hartley: layout and EMC talks](https://www.youtube.com/results?search_query=rick+hartley+pcb+layout)** (free) - The reference talks on ground planes, return currents and crosstalk.
- [Altium Academy / Zach Peterson](https://resources.altium.com/) (free) - PCB design articles and videos.
- [Phil's Lab](https://www.youtube.com/@PhilsLab) (free) - Modern PCB design (STM32, ESP32, RF), very educational.
- [Robert Feranec (FEDEVEL)](https://fedevel.education/) (free and paid) - Design reviews and workshops.
- [Eurocircuits: Design Guidelines](https://www.eurocircuits.com/) (free) - Design and manufacturing rules (DFM).
- [Sierra Circuits: PCB Design Guides](https://www.protoexpress.com/) (free) - Detailed guides on materials, stackups, impedances.
- [TI PCB Design Guidelines](https://www.ti.com/) (free) - Layout application notes by device family.
- [Analog Devices: PCB layout notes](https://www.analog.com/) (free) - Analog layout, decoupling, grounding.
- [Interference Technology](https://www.interferencetechnology.com/) (free) - EMC guides and articles, including low-cost pre-compliance.
- [JLCPCB: Impedance Calculator](https://jlcpcb.com/pcb-impedance-calculator) (free) - Stackups and impedances matched to their process.

### PCB Fabrication and Assembly

- **[JLCPCB](https://jlcpcb.com/)** (paid) - Very cheap prototypes, SMT assembly with an LCSC parts library.
- [PCBWay](https://www.pcbway.com/) (paid) - Fabrication, assembly, 3D printing, machining.
- [OSH Park](https://oshpark.com/) (paid) - Purple PCBs, community service made in the United States.
- [Aisler](https://aisler.net/) (paid) - Prototypes made in Europe (Germany).
- [Eurocircuits](https://www.eurocircuits.com/) (paid) - European fabrication with DFM checking tools.
- [Seeed Fusion](https://www.seeedstudio.com/fusion.html) (paid) - Fabrication and assembly.
- [Elecrow](https://www.elecrow.com/) (paid) - Fabrication and kits.
- [MacroFab](https://www.macrofab.com/) (paid) - US assembly and on-demand production.
- [OSH Stencils](https://www.oshstencils.com/) (paid) - Solder paste stencils.

### Hardware as Code and CI

- [atopile](https://atopile.io/) (free) - Describe circuits in code, with version control and validation.
- [tscircuit](https://tscircuit.com/) (free) - Design circuits in React/TypeScript.
- [SKiDL](https://github.com/devbisme/skidl) (free) - Circuits in Python, netlist generation.
- [KiBot](https://github.com/INTI-CMNB/KiBot) (free) - Production pipelines (see above).
- GitHub Actions with KiCad - Run DRC/ERC and generate manufacturing files on every commit using KiBot or kicad-cli.

---

## Components and Sourcing

### Distributors

**International generalists**

- **[Digi-Key](https://www.digikey.com/)** (paid) - Very large stock, excellent parametric search and datasheets.
- **[Mouser](https://www.mouser.com/)** (paid) - Broad catalog of active components.
- [Farnell / Newark / element14](https://www.farnell.com/) (paid) - European/US distributor, good support, professional pricing.
- [RS Components](https://www.rs-online.com/) (paid) - Components and industrial tooling.
- [LCSC](https://www.lcsc.com/) (paid) - Very low-cost components, tied to JLCPCB.
- [TME](https://www.tme.eu/) (paid) - European distributor (Poland), fast delivery.
- [Reichelt](https://www.reichelt.com/) (paid) - German distributor, good for common components.
- [Conrad](https://www.conrad.fr/) (paid) - Components, tools and instruments for consumers and professionals.
- [Arrow](https://www.arrow.com/) / [Avnet](https://www.avnet.com/) (paid) - Major semiconductor distributors.

**Maker and module specialists**

- [Adafruit](https://www.adafruit.com/) / [SparkFun](https://www.sparkfun.com/) / [Pololu](https://www.pololu.com/) / [DFRobot](https://www.dfrobot.com/) / [Seeed Studio](https://www.seeedstudio.com/) (paid) - Modules, development boards, sensors.
- [Tindie](https://www.tindie.com/) (paid) - Marketplace for independent electronics creators.
- [Crowd Supply](https://www.crowdsupply.com/) (paid) - Crowdfunding for open hardware (iCEBreaker, LibreVNA and more).

**French-language shops**

- [GoTronic](https://www.gotronic.fr/) (FR) (paid) - French distributor of components, modules and kits.
- [Lextronic](https://www.lextronic.fr/) (FR) (paid) - Development boards, robotics, modules.
- [Kubii](https://www.kubii.com/) (FR) (paid) - Raspberry Pi and accessories.
- [Conrad France](https://www.conrad.fr/) (FR) (paid) - Wide choice for consumers and professionals.

### Search, Datasheets and Inventory

- **[Octopart](https://octopart.com/)** (free) - Component search engine, prices and availability across all distributors.
- [Kitspace BOM Builder](https://kitspace.org/) (free) - Turn a BOM into carts at several distributors.
- [InvenTree](https://inventree.org/) (free) - Open source inventory management (parts, suppliers, BOMs).
- [Part-DB](https://github.com/Part-DB/Part-DB-server) (free) - Open source component database.
- [PartsBox](https://partsbox.com/) (paid) - Browser-based inventory and BOM management.
- [Wikipedia: list of 7400-series ICs](https://en.wikipedia.org/wiki/List_of_7400-series_integrated_circuits) (free) - Quick reference for discrete logic.
- [Nexperia Logic](https://www.nexperia.com/) / [TI Logic](https://www.ti.com/) (free) - Logic family selection guides.
- [AllDatasheet](https://www.alldatasheet.com/) (free) - Datasheets for old and obsolete parts. Prefer the manufacturer's source when it exists.

> Beware of counterfeits: buy from authorized distributors, especially power semiconductors and recent microcontrollers.

---

## Analog Electronics

**Op-amps and basic circuits**

- [Op Amps For Everyone](https://www.ti.com/lit/an/slod006b/slod006b.pdf) (free) - TI's free reference.
- [Analog Devices: Op Amp Applications Handbook](https://www.analog.com/) (free) - Theory and applications of op-amps.
- [TI Analog Engineer's Circuit Cookbook](https://www.ti.com/) (free) - Step-by-step circuit designs (op-amps, ADCs, sensors).
- [Analog Devices: Circuits from the Lab](https://www.analog.com/) (free) - Tested and documented reference circuits.
- [Electronics Weekly Circuit Collection](https://www.electronicsweekly.com/) (free) - Engineers' circuits.

**Filters**

- [TI Filter Designer](https://www.ti.com/) (free) - Design active filters online.
- [Analog Devices Filter Wizard](https://www.analog.com/) (free) - Active filter and network design.
- [Okawa Electric Design calculators](http://sim.okawa-denshi.jp/en/Fkeisan.htm) (free) - Various filter calculators (Sallen-Key, MFB and more).

**Data conversion (ADC / DAC)**

- [Analog Devices: Data Conversion Handbook](https://www.analog.com/en/education/education-library.html) (free) - Reference book on converters.
- [TI Precision Labs: Data Converters](https://www.ti.com/) (free) - Video series on choosing and using converters.

**Noise, precision and references**

- [Analog Devices: op-amp noise](https://www.analog.com/) (free) - Noise modeling.
- [Marco Reps (metrology)](https://www.youtube.com/@marcoreps) (free) - Voltage references, very high precision measurements.
- [Linear Technology Application Notes](https://www.analog.com/) (free) - Notes by Jim Williams and colleagues (now at Analog Devices).

---

## Digital Electronics, Logic and FPGA

**Fundamentals**

- [Ben Eater](https://eater.net/) (free) - From transistor to processor.
- [Nand2Tetris](https://www.nand2tetris.org/) (free) - Build a computer from logic gates.
- [HDLBits](https://hdlbits.01xz.net/) (free) - Interactive Verilog exercises with simulation.
- [Nandland](https://nandland.com/) (free) - FPGA, VHDL and Verilog tutorials.
- [Project F](https://projectf.io/) (free) - FPGAs and graphics: from an LED to 2D/3D rendering.

**Languages**

- [Verilog / SystemVerilog](https://www.accellera.org/) - Accellera and IEEE 1800 standards.
- [VHDL](https://ieeexplore.ieee.org/) - IEEE 1076 standard.
- [Amaranth HDL](https://github.com/amaranth-lang/amaranth) (free) - Hardware description in Python.
- [Chisel](https://www.chisel-lang.org/) (free) - Hardware description in Scala.
- [SpinalHDL](https://spinalhdl.github.io/SpinalDoc-RTD/) (free) - Hardware description in Scala.
- [LiteX](https://github.com/enjoy-digital/litex) (free) - SoC generator for FPGAs.
- [Clash](https://clash-lang.org/) (free) - Hardware description in Haskell.

**Open source tools**

- **[Yosys](https://github.com/YosysHQ/yosys)** (free) - Open source logic synthesis.
- [nextpnr](https://github.com/YosysHQ/nextpnr) (free) - Place and route for iCE40, ECP5, Gowin and others.
- [OSS CAD Suite](https://github.com/YosysHQ/oss-cad-suite-build) (free) - Ready-to-use distribution of open source FPGA tools.
- [Verilator](https://www.veripool.org/verilator/) (free) - Very fast Verilog simulation.
- [Icarus Verilog](https://github.com/steveicarus/iverilog) (free) - Verilog simulator.
- [GHDL](https://github.com/ghdl/ghdl) (free) - VHDL simulator.
- [cocotb](https://www.cocotb.org/) (free) - Verify circuits in Python.
- [Digital](https://github.com/hneemann/Digital) / [Logisim-evolution](https://github.com/logisim-evolution/logisim-evolution) (free) - Logic simulation for teaching.

**Boards and vendors**

- [Lattice (iCE40, ECP5)](https://www.latticesemi.com/) - Families well supported by the open source toolchain.
- [iCEBreaker](https://www.crowdsupply.com/1bitsquared/icebreaker-fpga) - Open source iCE40 board for learning.
- [Gowin / Sipeed Tang Nano](https://www.gowinsemi.com/) - Very affordable FPGAs.
- [AMD (Xilinx) Artix / Zynq](https://www.amd.com/) - FPGAs and SoCs with a proprietary toolchain (Vivado).
- [Intel (Altera) Cyclone](https://www.intel.com/) - FPGAs with Quartus.
- [Digilent](https://digilent.com/) - Arty, Basys and Nexys boards for teaching.
- [MiSTer FPGA](https://github.com/MiSTer-devel/Main_MiSTer/wiki) - Platform for recreating retro consoles and home computers.

**Reference lists**

- [hdl/awesome](https://github.com/hdl/awesome) (free) - Tools, IP cores and libraries for HDL design and verification.
- [aolofsson/awesome-opensource-hardware](https://github.com/aolofsson/awesome-opensource-hardware) (free) - Open hardware tools and projects.

---

## Microcontrollers and Embedded Systems

**Platforms and SDKs**

- **[Arduino](https://www.arduino.cc/)** (free) - Entry-level ecosystem with a huge body of resources.
- **[Raspberry Pi Pico (RP2040 / RP2350)](https://www.raspberrypi.com/documentation/microcontrollers/)** (free) - Very high-quality documentation and SDK, unique PIO.
- [ESP32 / ESP-IDF (Espressif)](https://docs.espressif.com/) (free) - Low-cost Wi-Fi/Bluetooth, complete SDK.
- [STM32 (STMicroelectronics)](https://www.st.com/en/development-tools/stm32cubeide.html) (free) - STM32CubeIDE, broad ARM Cortex-M family.
- [Nordic nRF Connect SDK](https://www.nordicsemi.com/) (free) - BLE, Thread, Zigbee and Matter.
- [Microchip (AVR / PIC / SAM)](https://www.microchip.com/) (free) - AVR (ATmega) and PIC families.
- [WCH CH32V](https://www.wch-ic.com/) (free) - Very inexpensive RISC-V microcontrollers.
- [PlatformIO](https://platformio.org/) (free) - Cross-platform embedded development environment.
- [Espressif MCU Selector](https://espressif-search.techalchemy.fr/) (FR) (free) - Independent community tool to filter and compare 64 Espressif chips and modules (CPU, GPIO, memory, PCB layers, integration complexity), with a part-number decoder. Not affiliated with Espressif.

**Real-time operating systems**

- [Zephyr](https://www.zephyrproject.org/) (free) - Modern RTOS with very broad board support.
- [FreeRTOS](https://www.freertos.org/) (free) - Widely used RTOS.
- [RIOT](https://www.riot-os.org/) (free) - RTOS for IoT.
- [NuttX](https://nuttx.apache.org/) (free) - POSIX-compatible RTOS.

**Languages**

- [MicroPython](https://micropython.org/) / [CircuitPython](https://circuitpython.org/) (free) - Python on microcontrollers.
- [The Embedded Rust Book](https://docs.rust-embedded.org/book/) (free) - Embedded Rust.
- [Embassy](https://embassy.dev/) (free) - Async Rust framework for microcontrollers.
- [probe-rs](https://probe.rs/) (free) - Vendor-independent debugging and flashing in Rust.
- [TinyGo](https://tinygo.org/) (free) - Go for microcontrollers.

**Debugging and tools**

- [OpenOCD](https://openocd.org/) (free) - Open source JTAG/SWD debugging.
- [Black Magic Probe](https://black-magic.org/) (free) - Debugger with a built-in GDB server.
- [sigrok / PulseView](https://sigrok.org/) (free) - Protocol analysis (I2C, SPI, UART, CAN and more).
- [SEGGER](https://www.segger.com/) - J-Link, RTT and SystemView.

**Learning embedded**

- [Interrupt (Memfault)](https://interrupt.memfault.com/) (free) - In-depth embedded engineering blog.
- [Embedded Artistry](https://embeddedartistry.com/) (free) - Firmware design best practices.
- [Embedded.fm](https://embedded.fm/) (free) - The reference podcast.
- [Beyond Logic: USB in a NutShell](https://www.beyondlogic.org/usbnutshell/usb1.shtml) (free) - Understand USB.
- [NXP UM10204: I2C specification](https://www.nxp.com/docs/en/user-guide/UM10204.pdf) (free) - The official I2C bus specification.
- [tinyML Foundation](https://www.tinyml.org/) (free) - Machine learning on microcontrollers.

**Related awesome lists**

- [rust-embedded/awesome-embedded-rust](https://github.com/rust-embedded/awesome-embedded-rust) - Embedded Rust.
- [mcauser/awesome-micropython](https://github.com/mcauser/awesome-micropython) - MicroPython.
- [agucova/awesome-esp](https://github.com/agucova/awesome-esp) - ESP8266 / ESP32.

---

## Power Electronics, Power Supplies and Batteries

> **Safety warning**: any electronics connected to the mains can kill. Use an isolation transformer and suitable probes, never work alone on mains-powered circuits, and respect creepage and clearance distances.

**Switching supplies and regulation**

- **[TI Power Tips](https://www.ti.com/)** (free) - Practical power supply design tips.
- [Analog Devices: LTpowerCAD / LTpowerPlanner](https://www.analog.com/) (free) - Power design and planning.
- [Wurth REDEXPERT](https://www.we-online.com/en/components/redexpert) (free) - Inductor and capacitor losses.
- [Ridley Engineering](https://www.ridleyengineering.com/) (free) - Articles on power supply control loops.
- [Biricha Digital](https://biricha.com/) (free and paid) - Courses and tools for control loops (compensation).
- [Infineon Power Design Tools](https://www.infineon.com/) (free) - Converter sizing.
- [onsemi Power Supply Tools](https://www.onsemi.com/) (free) - Tools and application notes.

**Power semiconductors**

- [Efficient Power Conversion (EPC)](https://epc-co.com/) (free) - GaN, application notes.
- [Wolfspeed / Infineon / ROHM SiC](https://www.wolfspeed.com/) (free) - Silicon carbide (SiC) design resources.
- [Nexperia Application Handbook](https://www.nexperia.com/) (free) - Power MOSFETs and diodes.

**Batteries and energy management**

- **[Battery University](https://batteryuniversity.com/)** (free) - Battery chemistry and usage.
- [TI Battery Management Guide](https://www.ti.com/) (free) - Chargers, fuel gauges, protection.
- [Analog Devices: Battery Management](https://www.analog.com/) (free) - Cell monitoring and balancing.
- Warning: lithium cells are dangerous if charged incorrectly or short-circuited. Use protection circuits and a suitable charger.

**Motors and control**

- [SimpleFOC](https://simplefoc.com/) (free) - Open source field-oriented control (FOC) for BLDC motors.
- [VESC Project](https://vesc-project.com/) (free) - Open source motor controller (e-bikes, robots).
- [ODrive](https://odriverobotics.com/) - High-performance motor control.
- [Trinamic / Analog Devices](https://www.analog.com/) - Silent stepper motor drivers.

---

## RF, Antennas, SDR and Signal Processing

**Fundamentals and references**

- **[Microwaves101](https://www.microwaves101.com/)** (free) - Encyclopedia of microwave engineering.
- [RF Cafe](https://www.rfcafe.com/) (free) - RF resources, calculators, history.
- [Rohde & Schwarz: Learning Center](https://www.rohde-schwarz.com/) (free) - Application notes on RF and EMC measurements.
- [Keysight Application Notes](https://www.keysight.com/) (free) - RF measurement and design notes.
- [Analog Devices: RF & Microwave](https://www.analog.com/) (free) - RF system design notes.

**Amateur radio**

- [ARRL](https://www.arrl.org/) (free and paid) - The worldwide amateur radio reference (*ARRL Handbook*).
- [REF: Reseau des Emetteurs Francais](https://www.r-e-f.org/) (FR) (free) - French amateur radio association.
- [w2aew (Alan Wolke)](https://www.youtube.com/@w2aew) (free) - Measurement, RF and amateur radio videos.

**Antennas**

- [4nec2](https://www.qsl.net/4nec2/) / [xnec2c](https://github.com/KJ7LNW/xnec2c) (free) - Antenna modeling.
- [openEMS](https://openems.de/) (free) - Electromagnetic simulation of planar structures and antennas.
- [scikit-rf](https://scikit-rf.org/) (free) - S-parameter processing in Python.

**SDR (software-defined radio)**

- **[PySDR](https://pysdr.org/)** (free) - Practical guide to SDR and DSP in Python.
- [GNU Radio](https://www.gnuradio.org/) (free) - Block-based signal processing environment.
- [RTL-SDR Blog](https://www.rtl-sdr.com/) (free) - Very low-cost SDR receiver and tutorials.
- [HackRF (Great Scott Gadgets)](https://greatscottgadgets.com/hackrf/) - Open SDR transceiver.
- [SDRangel](https://github.com/f4exb/sdrangel) (free) - SDR application with many modes.
- [ADALM-PLUTO](https://www.analog.com/) - Analog Devices' learning SDR.

**Wireless protocols**

- [Semtech LoRa](https://www.semtech.com/lora) (free) - LoRa and LoRaWAN documentation.
- [Nordic DevZone](https://devzone.nordicsemi.com/) (free) - BLE, Thread and Zigbee forum and docs.
- [Bluetooth SIG Specifications](https://www.bluetooth.com/specifications/) (free) - Official specifications.
- [u-blox Documentation](https://www.u-blox.com/) (free) - GNSS and wireless modules.

---

## Audio, Synthesizers and Instruments

- **[ESP: Elliott Sound Products](https://sound-au.com/)** (free) - Rod Elliott's projects and articles on analog audio.
- [DIY Audio](https://www.diyaudio.com/) (free) - The reference forum for homemade audio.
- [ElectroSmash](https://www.electrosmash.com/) (free) - Detailed analysis of effects and guitar amp circuits.
- [DIY Stompboxes](https://www.diystompboxes.com/) (free) - Effects pedal forum.
- [Beavis Audio](https://www.beavisaudio.com/) (free) - Audio circuit schematics and notes.
- [pichenettes/eurorack (Mutable Instruments)](https://github.com/pichenettes/eurorack) (free) - Open source code and designs for Eurorack modules.
- [Music From Outer Space](https://musicfromouterspace.com/) (free) - DIY analog synthesizer projects.
- [Sonelec Musique](https://www.sonelec-musique.com/) (FR) (free) - Audio and musical electronics in French.
- *Audio Power Amplifier Design* (Douglas Self) - Reference on amplifiers.

---

## Test and Measurement Equipment

**Basic equipment to own**

1. A reliable multimeter ([Fluke](https://www.fluke.com/), [Brymen](https://www.brymen.com/), [Keysight](https://www.keysight.com/), UNI-T).
2. A current-limited bench power supply ([Rigol](https://www.rigol.com/), [Siglent](https://www.siglent.com/), Korad).
3. An oscilloscope ([Rigol](https://www.rigol.com/), [Siglent](https://www.siglent.com/), [Keysight](https://www.keysight.com/), [Tektronix](https://www.tek.com/), [PicoScope](https://www.picotech.com/)).
4. A logic analyzer ([Saleae](https://www.saleae.com/), [DSLogic](https://www.dreamsourcelab.com/), sigrok-compatible clones).
5. A soldering station and a magnifier or microscope ([Soldering](#soldering-assembly-and-mechanics)).

**USB and learning instruments**

- [Digilent Analog Discovery](https://digilent.com/) (paid) - Scope, generator, power supply and logic analyzer in one USB box.
- [Analog Devices ADALM2000](https://www.analog.com/en/resources/evaluation-hardware-and-software/evaluation-boards-kits/adalm2000.html) (paid) - Portable learning instrument.
- [PicoScope](https://www.picotech.com/) (paid) - Professional-grade USB oscilloscopes.
- [Saleae](https://www.saleae.com/) (paid) - Very ergonomic USB logic analyzers.

**Measurement and analysis software**

- [sigrok / PulseView](https://sigrok.org/) (free) - Acquisition and protocol decoding on many devices.
- [PyVISA](https://pyvisa.readthedocs.io/) (free) - Programmatic instrument control (SCPI).
- [sigrok decoders](https://sigrok.org/wiki/Protocol_decoders) (free) - I2C, SPI, UART, CAN, USB decoders and more.

**RF and radio**

- [LibreVNA](https://github.com/jankae/LibreVNA) (free) - Open source vector network analyzer.
- [NanoVNA](https://nanovna.com/) - Very affordable portable VNA.
- [tinySA](https://tinysa.org/) - Small, economical spectrum analyzer.
- [RTL-SDR](https://www.rtl-sdr.com/) - Low-cost wideband SDR receiver.

**Learning to measure**

- [Tektronix: XYZs of Oscilloscopes](https://www.tek.com/) (free) - Introduction to oscilloscopes (search for "XYZs of Oscilloscopes").
- [Keysight: Oscilloscope Probing](https://www.keysight.com/) (free) - Notes on probes, bandwidth and loading.
- [EEVblog](https://www.eevblog.com/) (free) - Tutorials and instrument reviews (Dave Jones' channel).
- [w2aew](https://www.youtube.com/@w2aew) (free) - Measurements, probes, good practice.
- [Applied Science](https://www.youtube.com/@AppliedScience) (free) - Laboratory experiments and instrument building.

---

## Soldering, Assembly and Mechanics

**Soldering equipment**

- **[Pinecil (Pine64)](https://pine64.org/)** (paid) - Open source USB-C/DC soldering iron with excellent value for money.
- [JBC](https://www.jbctools.com/) / [Hakko](https://www.hakko.com/) / [Weller](https://www.weller-tools.com/) / [Metcal](https://www.metcal.com/) (paid) - Professional stations.
- [Miniware TS101](https://www.miniware.com.cn/) (paid) - Compact portable iron.
- Hot air station and reflow oven (T-962, hot plate) for SMD work (paid).

**Learning**

- [Soldering Is Easy](https://mightyohm.com/blog/2011/04/soldering-is-easy-comic-book-downloads/) (free) - Educational comic.
- [Adafruit: Guide to Excellent Soldering](https://learn.adafruit.com/adafruit-guide-excellent-soldering) (free) - Illustrated guide.
- [SparkFun: How to Solder](https://learn.sparkfun.com/) (free) - Through-hole and SMD soldering tutorials.
- [Pace Worldwide soldering videos](https://www.youtube.com/results?search_query=pace+soldering+tutorial) (free) - Professional soldering and rework videos (NASA/IPC references).
- [Dave Jones (EEVblog): SMD soldering tutorials](https://www.eevblog.com/) (free) - Soldering fine-pitch parts, QFN, BGA.

**Enclosures and mechanics**

- [FreeCAD](https://www.freecad.org/) (free) - Open source CAD, with KiCad StepUp for import.
- [OpenSCAD](https://openscad.org/) (free) - Parametric CAD by code.
- [Autodesk Fusion](https://www.autodesk.com/products/fusion-360/) (paid) - CAD with integrated electronics.
- [Hammond](https://www.hammfg.com/) / [Bud Industries](https://www.budind.com/) / [Takachi](https://www.takachi-el.co.jp/) (paid) - Standard enclosures.
- [Misumi](https://www.misumi-ec.com/) (paid) - Standard mechanical parts.
- 3D printing and laser cutting: see the [fablabs](#french-language-resources) near you.

---

## Troubleshooting, Repair and Reverse Engineering

- **[iFixit](https://www.ifixit.com/)** (free) - Repair guides and teardowns.
- [EEVblog Teardowns](https://www.eevblog.com/) (free) - Teardowns and design analysis.
- [Big Clive](https://www.youtube.com/@bigclive) (free) - Teardowns of inexpensive products and schematic analysis.
- [Mr Carlson's Lab](https://www.youtube.com/@MrCarlsonsLab) (free) - Restoring vintage electronics.
- [Louis Rossmann](https://www.youtube.com/@rossmanngroup) / [NorthridgeFix](https://www.youtube.com/@NorthridgeFix) (free) - Board-level repair (computers, consoles).
- [Learn Electronics Repair](https://www.youtube.com/@LearnElectronicsRepair) (free) - Repair without schematics.
- [Kerry Wong](https://www.kerrywong.com/) (free) - Blog and videos on measurement and analysis.
- [Ken Shirriff: Blog](https://www.righto.com/) (free) - Reverse engineering of integrated circuits and historical hardware.
- [Siliconpr0n](https://siliconpr0n.org/) (free) - Microscope photographs of chips.
- [Zeptobars](https://zeptobars.com/) (free) - Photographs of decapped silicon.
- [Badcaps Forum](https://www.badcaps.net/) (free) - Repairing failed capacitors and power supplies.
- *How to Diagnose and Fix Everything Electronic* - Michael Geier (book).

> Repair is also an excellent way to learn: you read the schematic, measure, replace, and understand why things fail.

---

## Hardware Security

> Practice only on hardware you own or with explicit authorization.

- ***The Hardware Hacking Handbook*** (paid) - Reference on side-channel and fault injection attacks.
- [ChipWhisperer (NewAE)](https://www.newae.com/chipwhisperer) - Learning platform for side-channel attacks and glitching.
- [Ghidra](https://github.com/NationalSecurityAgency/ghidra) (free) - Firmware reverse engineering.
- [Glasgow Interface Explorer](https://glasgow-embedded.org/) (free) - Universal hardware interface tool.
- [Bus Pirate](https://buspirate.com/) (free) - Interface with I2C, SPI, UART and JTAG chips.
- [OpenOCD](https://openocd.org/) (free) - JTAG/SWD access.
- [Joe Grand](https://www.grandideastudio.com/) (free) - Hardware security projects and training.
- [bunnie Huang: Bunnie Studios](https://www.bunniestudios.com/) (free) - Blog on hardware design and security.
- [Flipper Zero](https://flipperzero.one/) (paid) - Multi-protocol learning tool (RFID, infrared, sub-GHz and more).

---

## Open Source Silicon (Chip Design)

> Designing an integrated circuit is now accessible with fully open source tools and multi-project "shuttles".

**Quick start**

- **[Tiny Tapeout](https://tinytapeout.com/)** - Get your own digital or mixed-signal design manufactured on the SkyWater 130 nm process. Recent runs (for example TTSKY26b, launched in April 2026) are produced through ChipFoundry shuttles.
- [Zero to ASIC Course](https://zerotoasiccourse.com/) - Course to design and manufacture a chip with open source tools.
- [wafer.space](https://wafer.space/) - Open source silicon shuttles on GlobalFoundries' GF180MCU PDK (180 nm).
- [ChipFoundry](https://chipfoundry.io/) - Continuation of open source shuttle activity after Efabless closed (March 2025), on SkyWater 130 nm.

**Tools (RTL to GDSII flow)**

- **[OpenROAD](https://theopenroadproject.org/)** (free) - Automated place and route, used in several hundred tapeouts.
- [LibreLane](https://github.com/librelane/librelane) (free) - Flow orchestration (successor to OpenLane).
- [Yosys](https://github.com/YosysHQ/yosys) (free) - Logic synthesis.
- [OpenSTA](https://github.com/The-OpenROAD-Project/OpenSTA) (free) - Static timing analysis.
- [Magic](http://opencircuitdesign.com/magic/) (free) - Layout editor and DRC.
- [KLayout](https://www.klayout.de/) (free) - Layout viewing and verification.
- [Netgen](http://opencircuitdesign.com/netgen/) (free) - LVS (Layout vs. Schematic).
- [Xschem](https://xschem.sourceforge.io/) (free) - Schematic capture for analog/CMOS circuits.
- [ngspice](https://ngspice.sourceforge.io/) (free) - Analog and mixed-signal circuit simulation.

**Open process design kits (PDKs)**

- [SkyWater SKY130](https://github.com/google/skywater-pdk) (free) - 130 nm, the first open foundry PDK.
- [GlobalFoundries GF180MCU](https://github.com/google/gf180mcu-pdk) (free) - 180 nm, mixed-signal.
- [IHP Open PDK (SG13G2)](https://github.com/IHP-GmbH/IHP-Open-PDK) (free) - 130 nm SiGe BiCMOS for RF and high frequency.

**Community and architecture**

- [FOSSi Foundation](https://fossi-foundation.org/) - Foundation for free and open source silicon.
- [CHIPS Alliance](https://www.chipsalliance.org/) - Open source collaboration around hardware.
- [RISC-V International](https://riscv.org/) - Open instruction set architecture.
- [OpenTitan](https://opentitan.org/) - Open source root of trust.
- [hdl/awesome](https://github.com/hdl/awesome) - List of HDL and ASIC tools.

---

## Home Automation, IoT and Robotics

- [ESPHome](https://esphome.io/) (free) - Configurable firmware for ESP32 and ESP8266, tied to Home Assistant.
- [Home Assistant](https://www.home-assistant.io/) (free) - Local home automation platform.
- [Tasmota](https://tasmota.github.io/docs/) (free) - Alternative firmware for smart plugs and modules.
- [Zigbee2MQTT](https://www.zigbee2mqtt.io/) (free) - Cloud-free Zigbee gateway.
- [Matter / Thread](https://csa-iot.org/) - Interoperable smart home standards.
- [MQTT](https://mqtt.org/) (free) - IoT messaging protocol.
- [Node-RED](https://nodered.org/) (free) - Flow-based automation.
- [ROS 2](https://docs.ros.org/) / [micro-ROS](https://micro.ros.org/) (free) - Robotics, including on microcontrollers.
- [Klipper / Marlin](https://www.klipper3d.org/) (free) - 3D printer firmware (applied embedded electronics).
- [Framboise 314](https://framboise314.fr/) (FR) (free) - French-language blog on Raspberry Pi and micro-computing.

---

## Standards, Compliance and Regulation

> To sell an electronic product in Europe, you must demonstrate compliance with the applicable directives (CE marking).

**Main European texts** (available on [EUR-Lex](https://eur-lex.europa.eu/))

- EMC Directive 2014/30/EU (electromagnetic compatibility).
- Low Voltage Directive 2014/35/EU.
- RED Directive 2014/53/EU (radio equipment).
- RoHS Directive 2011/65/EU (hazardous substances).
- WEEE Directive 2012/19/EU (waste electrical and electronic equipment).
- REACH Regulation (chemical substances).

**Standards and organizations**

- [IPC](https://www.ipc.org/) (paid) - PCB design, manufacturing and acceptance standards (IPC-2221, IPC-A-610, J-STD-001 and more).
- [IEC](https://www.iec.ch/) (paid) - International standards (IEC 62368-1 for audio/video and ICT equipment safety).
- [JEDEC](https://www.jedec.org/) (paid) - Semiconductor and memory standards.
- [IEEE Standards](https://standards.ieee.org/) (paid) - IEEE standards.
- [USB-IF](https://www.usb.org/) (free) - USB specifications.
- [NXP UM10204 (I2C)](https://www.nxp.com/docs/en/user-guide/UM10204.pdf) (free) - I2C specification.
- [CAN in Automation](https://www.can-cia.org/) (free) - CAN and CANopen documentation.

**Practical compliance**

- [Interference Technology](https://www.interferencetechnology.com/) (free) - EMC guides and articles, including low-budget pre-compliance.
- [Rohde & Schwarz: EMC Fundamentals](https://www.rohde-schwarz.com/) (free) - Application notes on EMC testing.
- [Wurth Elektronik: design resources](https://www.we-online.com/) (free) - *Trilogy of Magnetics* (design book on magnetic components) and notes on EMC filtering.

---

## Open Source Hardware

- **[OSHWA: Open Source Hardware Association](https://www.oshwa.org/)** (free) - Definition and certification of open hardware.
- [Hackaday.io](https://hackaday.io/) (free) - Platform for documented projects.
- [Kitspace](https://kitspace.org/) (free) - Share PCB projects with an order-ready BOM.
- [OSH Park Shared Projects](https://oshpark.com/shared_projects) (free) - Shared PCBs you can order in one click.
- [Crowd Supply](https://www.crowdsupply.com/) - Crowdfunding platform for open hardware.
- [Open Source Ecology](https://www.opensourceecology.org/) (free) - Open machines.
- [GitHub topic: open-source-hardware](https://github.com/topics/open-source-hardware) (free) - Open hardware projects.
- [aolofsson/awesome-opensource-hardware](https://github.com/aolofsson/awesome-opensource-hardware) (free) - List of tools and projects.

---

## Videos, Podcasts, Blogs and Magazines

**YouTube channels (English)**

- **[EEVblog](https://www.eevblog.com/)** - Dave Jones: design, teardowns, measurement, answers to beginner questions.
- **[GreatScott!](https://www.youtube.com/@greatscottlab)** - Accessible projects and explanations.
- [ElectroBOOM](https://www.youtube.com/@ElectroBOOM) - Physics and electronics with humor.
- [Afrotechmods](https://www.youtube.com/@afrotechmods) - Short, clear tutorials.
- [w2aew](https://www.youtube.com/@w2aew) - Measurements, RF and outstanding teaching.
- [Andreas Spiess](https://www.youtube.com/@AndreasSpiess) - ESP32, sensors, IoT.
- [Ben Eater](https://eater.net/) - From transistor to CPU.
- [Phil's Lab](https://www.youtube.com/@PhilsLab) - Modern PCB and firmware design.
- [Robert Feranec](https://fedevel.education/) - PCB design reviews.
- [Big Clive](https://www.youtube.com/@bigclive) - Teardowns of inexpensive products.
- [Mr Carlson's Lab](https://www.youtube.com/@MrCarlsonsLab) - Restoration and circuits.
- [Julian Ilett](https://www.youtube.com/@JulianIlett) - Electronics and embedded projects.
- [Jeremy Blum](https://www.jeremyblum.com/) - Electronics, Arduino, design.
- [Voltlog](https://www.youtube.com/@Voltlog) - Reviews and projects.
- [Marco Reps](https://www.youtube.com/@marcoreps) - Metrology and references.
- [Kerry Wong](https://www.kerrywong.com/) - Measurement and analysis.
- [Applied Science](https://www.youtube.com/@AppliedScience) - Experiments and instruments.
- [The Signal Path](https://www.youtube.com/@TheSignalPath) - RF measurements and circuit analysis.
- [Contextual Electronics](https://contextualelectronics.com/) - Product design.
- [Altium Academy](https://www.youtube.com/@AltiumAcademy) - PCB design.
- [SparkFun](https://www.youtube.com/@SparkFun) / [Adafruit](https://www.youtube.com/@adafruit) / [DigiKey](https://www.youtube.com/@digikey) - Tutorials and news.
- [Texas Instruments](https://www.youtube.com/@TexasInstruments) / [Analog Devices](https://www.youtube.com/@AnalogDevicesInc) - Manufacturer training.
- [Hackaday](https://www.youtube.com/@Hackaday) - Projects and Supercon talks.

**French-language channels**

French-language electronics channels change quickly. To avoid publishing unverified links, this section is deliberately left open: **community contributions are welcome** (see [Contributing](#contributing)).

**Podcasts**

- [The Amp Hour](https://theamphour.com/) (free) - Electronics podcast by engineers.
- [Embedded.fm](https://embedded.fm/) (free) - Interviews on embedded systems.
- [Hackaday Podcast](https://hackaday.com/) (free) - Weekly hacker news.
- [Signal Integrity Journal](https://www.signalintegrityjournal.com/) (free) - Signal integrity.

**Blogs and news sites**

- **[Hackaday](https://hackaday.com/)** (free) - Hacker and engineer projects every day.
- [Hackster.io](https://www.hackster.io/) (free) - Projects and news.
- [EDN](https://www.edn.com/) / [EE Times](https://www.eetimes.com/) / [Electronic Design](https://www.electronicdesign.com/) / [Electronics Weekly](https://www.electronicsweekly.com/) (free) - Trade press.
- [Adafruit Blog](https://blog.adafruit.com/) / [SparkFun Blog](https://www.sparkfun.com/) (free) - Maker news.
- [Dangerous Prototypes](https://dangerousprototypes.com/) (free) - Open hardware projects.
- [Jeff Geerling](https://www.jeffgeerling.com/) (free) - Raspberry Pi, hardware and reviews.
- [Ken Shirriff](https://www.righto.com/) (free) - Chip reverse engineering.

**Magazines**

- [Elektor](https://www.elektormagazine.com/) (paid) - Projects and articles (French edition: [elektormagazine.fr](https://www.elektormagazine.fr/)).
- [Circuit Cellar](https://www.circuitcellar.com/) (paid) - Embedded and design.
- [Make:](https://makezine.com/) (paid) - Makers and projects.
- [Nuts & Volts](https://www.nutsvolts.com/) (paid) - Electronics and projects.
- [Silicon Chip](https://www.siliconchip.com.au/) (paid) - Australian electronics magazine.
- [Hackable / Editions Diamond](https://connect.ed-diamond.com/) (FR) (paid) - French magazine on open hardware and software projects.

---

## Communities and Forums

- **[EEVblog Forum](https://www.eevblog.com/forum/)** (free) - Forum full of experienced engineers.
- **[Electronics Stack Exchange](https://electronics.stackexchange.com/)** (free) - Technical Q&A.
- [Reddit: r/electronics](https://www.reddit.com/r/electronics/) / [r/AskElectronics](https://www.reddit.com/r/AskElectronics/) / [r/diyelectronics](https://www.reddit.com/r/diyelectronics/) (free) - General communities.
- [Reddit: r/PrintedCircuitBoard](https://www.reddit.com/r/PrintedCircuitBoard/) (free) - Community PCB reviews.
- [Reddit: r/embedded](https://www.reddit.com/r/embedded/) / [r/FPGA](https://www.reddit.com/r/FPGA/) (free) - Embedded and FPGA.
- [KiCad Forum](https://forum.kicad.info/) (free) - KiCad support.
- [All About Circuits Forum](https://forum.allaboutcircuits.com/) (free) - Help for beginners and intermediate users.
- [Arduino Forum](https://forum.arduino.cc/) (free) - Arduino support.
- [Raspberry Pi Forums](https://forums.raspberrypi.com/) (free) - Raspberry Pi and Pico support.
- [Hackaday.io](https://hackaday.io/) (free) - Projects and discussions.
- [Hackaday Supercon](https://hackaday.com/) (free) - Annual hacker conference.
- [DIY Audio](https://www.diyaudio.com/) (free) - Audio forum.
- [QRZ](https://www.qrz.com/) (free) - Amateur radio community.

---

## French-Language Resources

**Making spaces (France)**

- [Electrolab (Nanterre)](https://electrolab.fr/) (FR) (free) - Hackerspace in the Paris region.
- [Tetalab (Toulouse)](https://tetalab.org/) (FR) (free) - Hackerspace in Toulouse.
- [FabLabs.io](https://fablabs.io/) (free) - Worldwide fablab directory, with many French entries.
- [Hackerspaces.org](https://hackerspaces.org/) (free) - Worldwide hackerspace directory.

**French-language sites and forums**

- [Futura-Sciences forum: Electronique](https://forums.futura-sciences.com/electronique/) (FR) (free) - General French-language forum.
- [Zeste de Savoir](https://zestedesavoir.com/) (FR) (free) - French-language tutorials.
- [Locoduino](https://www.locoduino.org/) (FR) (free) - Arduino and model railways.
- [Eskimon](https://eskimon.fr/) (FR) (free) - Arduino for beginners.
- [Framboise 314](https://framboise314.fr/) (FR) (free) - Raspberry Pi.
- [ABC Electronique](https://www.abcelectronique.com/) (FR) (free) - Courses and schematics.
- [Sonelec Musique](https://www.sonelec-musique.com/) (FR) (free) - Audio and music.
- [FUN MOOC](https://www.fun-mooc.fr/) (FR) (free) - Online courses.
- [Elektor France](https://www.elektormagazine.fr/) (FR) (paid) - Magazine and books in French.
- [GoTronic](https://www.gotronic.fr/) / [Lextronic](https://www.lextronic.fr/) / [Kubii](https://www.kubii.com/) (FR) (paid) - French component and module shops.

---

## Other Awesome Lists

- [kitspace/awesome-electronics](https://github.com/kitspace/awesome-electronics) - The reference English-language list (thousands of GitHub stars).
- [techgaun/awesome-electronics](https://github.com/techgaun/awesome-electronics) - Personal list of DIY resources.
- [hdl/awesome](https://github.com/hdl/awesome) - HDL design and verification.
- [rust-embedded/awesome-embedded-rust](https://github.com/rust-embedded/awesome-embedded-rust) - Embedded Rust.
- [mcauser/awesome-micropython](https://github.com/mcauser/awesome-micropython) - MicroPython.
- [agucova/awesome-esp](https://github.com/agucova/awesome-esp) - ESP8266 / ESP32.
- [aolofsson/awesome-opensource-hardware](https://github.com/aolofsson/awesome-opensource-hardware) - Open hardware.
- [sindresorhus/awesome](https://github.com/sindresorhus/awesome) - The list of all awesome lists.

---

## Contributing

Contributions are welcome, especially for:

- **French-language resources** (YouTube channels, courses, forums, shops);
- **broken or outdated links** (report them with the date);
- **areas to deepen** (EMC, medical, automotive, space, photovoltaics, precision analog electronics).

**Simple rules**

1. One line per resource: `- [Name](URL) (tags) - Short, factual description.`
2. Use the tags (FR), (free), (paid), (freemium) where they apply, and bold the name only for essential resources.
3. Put the resource in the right section and keep a logical order (essentials first).
4. Avoid duplicates and affiliate links.
5. Prefer primary sources (manufacturers, official documentation, authors) over aggregators.

---

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the author has waived all copyright and related rights to this list. Product and brand names belong to their respective owners.
