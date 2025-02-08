# Practice School 2025 Sem 8

- **PRE-REQS**:
  - Students with NO Linux exeperience may follow these [8 Lessons in Linux](https://github.com/silicon-vlsi-org/module-cs3-301) to get started.
  - If you haven't, install **Windows Subsystem for Linux (WSL)** on your Windows 10/11. **Follow this [page](https://github.com/silicon-vlsi-org/eda-wsl2)**
  - If you don't have one yet, create a [GitHub](https://github.com) account.
    - Create a Git Repository with the name `PS-2025-S8-<username>` where, username is First initial and Surname or Surname Initial and First Name. For eg. if name is _Subash Bose_, the repossitory name should be `PS-2025-S8-sbose`

# Resources

- **TEXT**
  - [**Hodges**] D.A., et.al., "_Analysis and Design of Digital Integrated Circuits_", Tata-McGraw Hill, 3rd Ed
  - [**Rout**], Saroj. 2025. IC Engineering I. [[eBook](https://mixignal-press.github.io/ebook-ice1/)]
    - Most of the notes covered during this PS will shared on this eBook.
- **REFERENCES**
  - [**Kang**] S., Leblebici and Kim C., "_CMOS Digital Integrated Circuits_, McGraw Hill, 4th Ed, 2015.
  - [**Weste**] Weste, Neil, and David Harris. "*CMOS VLSI Design: A Circuits and Systems Perspective*". Pearson Education, 2011
  - [**Thomas**], R. E., Rosa, A. J., Toussaint, G. J. (2023). _The Analysis and Design of Linear Circuits_. United Kingdom: Wiley. [Thomas2023]
  - [**Sadiku**] M.N.O and Alexander C.K., _Fundamentals of Electric Circuits_. McGraw-Hill Higher Education, 2007. [[Online](https://archive.org/details/sadiku-fundamentals-of-electric-circuits-6th-2016)]
  - [**Uyemura**] Uyemura, John P. "*CMOS Logic Circuit Design*". Springer, 2007
  - [**Baker**] Baker, R. Jacob. "*CMOS: Circuit Design, Layout, and Simulation*". John Wiley & Sons, 2008

- **VIRTUAL LABS**
  - [PhET](https://phet.colorado.edu/en/simulations/filter?subjects=physics&type=html): University of Colorado
  - [VLAB](https://www.laboratoriovirtual.fisica.ufc.br/capacitores?lang=en): at Federal University of Ceara. This is a good for doing measurements with multimeters.
    
# EE Refresher

- **PASSIVE DEVICES**: Resistor, Capacitor and Inductors (RLC)  [[Chap-2: Passives](https://mixignal-press.github.io/ebook-ice1/passives.html)] [[Video-2021](https://www.youtube.com/watch?v=3SCYAH57Ixw)
   - Derivation of IV char for resistive material.
   - Derivation of Capacitance using Gauss's Law.
   - Basic inductance calculation.
- **BASIC CIRCUIT THEORY** [[Chap-3: Linear Circuit](https://mixignal-press.github.io/ebook-ice1/circuits.html)] [Video-2021](https://www.youtube.com/watch?v=OzlsThjjUDA)
  - Basic circuit analysis: Voltage current division, circuit reduction.
  - Analysis techniques:
    - Node-voltage and mesh-analysis
    - Linearity properties
    - Thevenin and Norton equivalent.
    - Interface circuit design
  - **Reading Assignment**: Chap-2 and 3 from [Thomas2023]
  - **Problems**:
    - Basic Circuits: [Thomas2023] (2.2, 2.5, 2.7(a,b), 2.10, 2.25, 2.26, 2.27, 2.31, 2.34, 2.35, 2.37, 2.49, 2.50)
    - Circuit Analysis Techniques: [Thomas2023]
      - Node and Mesh Analysis: (3.1, 3.6, 3.8, 3.9, 3.11, 3.14)
      - Superposition: (3.33, 3.35, 3.36)
      - Thevenin and Norton: (3.39, 3.42, 3.45, 3.48, 3.52)
      - Maximum Power Transfer: (3.57, 3.59, 3.61)

# CMOS VLSI DESIGN

- **INTRODUCTION**
  - Introduction to CMOS VLSI Design Flow [[Video-2021](https://www.youtube.com/watch?v=NVzHuigvpt4)]]
    - [*Suggested Reading*]: [Hodges] Chapter-**1**, [Kang] (**Chapter-1.3-1.5**) (Just an overview reading is fine.)
- **CMOS PROCESSING**
  - Introduction to CMOS Processing [[Video-2021](https://www.youtube.com/watch?v=dauFDKM-Eu0)]
    - [*Highly Recomended*]: [Annotted Chapter from Weste-Harris and Johns-Martin](https://www.dropbox.com/s/zxp1dnwknvpfz8y/Weste-JohnsMartin-CMOSprocessing-Layout-Highlight-annotate.pdf)
    - [*Suggested Reading*]: [Hodges] Section **3.1,3.2**
    - [*Suggested Problems*]: [Hodges] Prob **3.11, 3.12**
- **MOS DEVICE**
  - Threshold Voltage (Vt) [[Video-2021](https://www.youtube.com/watch?v=OUZV9N0b3Lc)]
    - [*Suggested Reading*]: [Hodges] Section **3.2.4, 3.2.5**
    - [*Suggested Problems*]: [Hodges] Example **3.1**, Prob **3.13, 3.14**
  - IV Characteristics and MOS Capacitance. [[Video-2021](https://www.youtube.com/watch?v=UUCB_dgFiwA)]
    - [*Suggested Reading*]: [Hodges] Section **2.2.1, 2.2.2, 2.2.3, 2.2.7** [Kang]: Chapter **3** [Uyemura] Section **1.1, 1.2** (Excellent treatment on Vt) [Baker]: Section **6.1, 6.2, 6.3**
    - [*Suggested Problems*]: [Hodges] Example **2.1,2.2,2.3,2.4,2.5,2.11**, Prob. **2.1,2.4,2.5,2.7,2.8**
  - Modeling of MOS Device for Circuit Simulation.: [[Video-2021](https://www.youtube.com/watch?v=mQEryii3McE)]
    - [*Suggested Reading*]: [Hodges] Section **3.4, 3.5, 3.6, Appendix-A**, [NGSpice Manual]
    - [*Lab Assignment*] MOS Parameter extraction and MOS Level-1 Modeling [Link-to-PDK](docs/2021-0528-Assignment-MOS-SPICE.pdf) <-- FIXME
      - [[Video-2021](https://www.youtube.com/watch?v=zFpJc6QFUc4)]
- **INVERTER CHARACTERISTICS**
  - Static Inverter Characteristics [[Video-2021](https://www.youtube.com/watch?v=DJALnK61MYs)]
    - [*Suggested Reading*]: [Hodges] Chapter 4
    - [*Suggested Problems*]: [Hodges] Example **4.6**, Problem **4.1,4.2,4.5,4.8,4.10,4.11**
  - Dynamic Inverter Characteristics [[Video-2021](https://www.youtube.com/watch?v=jXyXVIjiYcU)]
    - [*Suggested Reading*]: [Hodges] Section **6.1,6.2,6.3,6.4,6.5**  
    - [*Suggested Problems*]: [Hodges] Example **6.1,6.3,6.4,6.5,6.8**

# Computer Aided Design and Automation

- Get your github repo cloned and synced in your WSL/Ubuntu account using SSH. 
- Get familiar with editor `vim`. 
  - As an exercise for `vim` and `git`, open your README.md and create a documentation for Capacitor section and insert a table with the capacitor properties.
- [Tutorial from Perplexity](https://www.perplexity.ai/search/create-a-quick-vim-editor-tuto-OOEC6K37R9a6DdMBq4TTew) : Short tutorials on `vim`, `git` and writing equations in markdown

* * *

[Thomas2023]:           https://www.dropbox.com/scl/fi/83ygnyynx2sfex1h7tdhg/Thomas-AnalysisDesignOfLinearCkts-Wiley-2023.pdf?rlkey=4xzk0an1z7r3fcj936o0enjg4&st=oio90ydk&dl=0
[SCMOS]:                https://www.mosis.com/files/scmos/scmos.pdf
[NGSpice]:              http://ngspice.sourceforge.net
[NGSpiceMan]:           http://ngspice.sourceforge.net/docs/ngspice-html-manual/manual.xhtml
[Magic]:                http://opencircuitdesign.com/magic/
[Netgen]:               http://opencircuitdesign.com/netgen/

