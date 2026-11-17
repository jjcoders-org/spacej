
# SPACEJ — AEROSPACE ENGINEERING RESEARCH

Version: 1.0
Research ID: RESEARCH-001
Started: 17 November 2026
Status: In Progress
Organisation: JJ Coders
Project: SpaceJ

---

# 1. RESEARCH OBJECTIVE

Understand existing aerospace engineering software, technologies, and data infrastructure before selecting SpaceJ's first engineering project.

We must understand what already exists, what problems these technologies solve, who uses them, and where potential opportunities might exist.

SpaceJ must not build a duplicate of an existing technology without a demonstrated reason.

This research investigates three important technologies:

1. NASA GMAT — General Mission Analysis Tool.
2. Basilisk — Astrodynamics Simulation Framework.
3. CelesTrak — Public satellite orbital data infrastructure.

The objective is to develop an initial technical understanding and identify questions for further investigation.

No commercial opportunity is considered validated merely because it appears interesting.

---

# 2. NASA GMAT — GENERAL MISSION ANALYSIS TOOL

## 2.1 Overview

Organisation: NASA and external contributors.

Official repository:
https://github.com/NASA/GMAT

Official documentation:
https://gmat.atlassian.net/wiki/spaces/GW/

NASA Software Catalog:
https://software.nasa.gov/software/GSC-19640-1

Latest release identified during this research:
R2026a — 6 May 2026.

## 2.2 What is GMAT?

GMAT is an open-source aerospace engineering application used for space mission design, navigation, optimisation, and analysis.

It allows engineers to create spacecraft mission scenarios, model orbital behaviour, analyse trajectories, and investigate mission requirements.

It supports mission environments ranging from low Earth orbit to lunar, libration-point, and deep-space missions.

GMAT can be operated through:
- A graphical user interface.
- Its own scripting language.
- Python programming environments.
- Java programming environments.

## 2.3 Problems GMAT solves

Space missions require extensive mathematical modelling and analysis.

Engineers need to understand:
- Where a spacecraft will travel.
- How its orbit changes.
- What manoeuvres are necessary.
- How a mission can reach its destination.
- How different mission parameters affect the outcome.

GMAT provides tools to model and analyse these problems.

## 2.4 Main capabilities

### Mission design
Create and analyse spacecraft mission scenarios.

### Orbital mechanics
Model and investigate spacecraft orbital behaviour.

### Trajectory optimisation
Study and optimise spacecraft trajectories and manoeuvres.

### Navigation
Support spacecraft navigation analysis and orbit determination.

### Propulsion modelling
Model impulsive manoeuvres and continuous-thrust scenarios.

### Visualisation
Display mission parameters, orbital behaviour, plots, and reports.

### Extensibility
Create customised mission scenarios and extend the software through its development interfaces.

## 2.5 Technical architecture

- Main implementation language: C++.
- Interface options: GUI and custom scripting.
- Programming environments: Python and Java interfaces.
- Licence: Apache License 2.0.
- Platforms: Windows, Linux, and macOS.
- Category: Mission design and engineering analysis.

The application has an object-oriented architecture and supports extensible components.

## 2.6 Who uses GMAT?

Its documented user communities include:
- Aerospace engineers.
- Mission analysts.
- NASA and other engineering organisations.
- Academic researchers.
- Students.
- Space mission developers.

NASA documentation identifies real mission-support, engineering-study, educational, and public-engagement uses.

## 2.7 Limitations and considerations

The following are areas requiring investigation rather than claims that GMAT is defective.

1. Its extensive engineering capabilities may require substantial prior knowledge.
2. Users need to understand orbital mechanics and mission modelling.
3. Complex mission workflows require careful configuration.
4. Integration and automation requirements may differ between organisations.
5. Particular user groups may need workflows beyond those they currently use.

GMAT is a mature engineering tool. SpaceJ must understand its existing capabilities before proposing alternatives.

## 2.8 What SpaceJ can learn

- Extensive scientific software can be open source.
- A graphical interface and scripting can serve different engineering users.
- Mathematical models should be configurable.
- Mission analysis requires reproducible calculations.
- Engineering tools benefit from documented assumptions and validation.
- Extensibility is important for specialist users.

## 2.9 Potential opportunities to investigate

These are research hypotheses, not validated market gaps.

- More accessible mission-analysis workflows for specific user groups.
- Specialised visualisation and reporting.
- Interoperability with other engineering tools.
- Simplified data preparation.
- Browser-based interfaces for particular mission-analysis tasks.
- Better integrations for specific existing workflows.

Before pursuing any opportunity, speak to actual GMAT users and establish whether the need exists.

## 2.10 Research conclusion

GMAT already provides substantial space mission design and analysis capabilities.

Building another general-purpose mission-design application would require a strong technical and commercial justification.

SpaceJ should investigate specialised problems rather than attempt to replicate GMAT.

Sources:

https://github.com/NASA/GMAT

https://software.nasa.gov/software/GSC-19640-1

https://gmat.atlassian.net/wiki/spaces/GW/

Research date: 17 November 2026.

---

# 3. BASILISK — ASTRODYNAMICS SIMULATION FRAMEWORK

## 3.1 Overview

Project: Basilisk.

Official website:
https://avslab.github.io/basilisk/

Official documentation:
https://avslab.github.io/basilisk/

GitHub organisation:
https://github.com/AVSLab

Developer organisations:
- University of Colorado Boulder — Autonomous Vehicle Systems Laboratory.
- Laboratory for Atmospheric and Space Physics.

Documented release identified during research: 2.12.2.

## 3.2 What is Basilisk?

Basilisk is an open-source spacecraft simulation framework designed for advanced aerospace engineering, astrodynamics research, and spacecraft system modelling.

Unlike a simple orbit viewer, Basilisk can simulate complex spacecraft behaviour.

It supports simulations of spacecraft dynamics, attitude, guidance, navigation, control, and interacting spacecraft subsystems.

It is designed for researchers and engineers who need configurable and repeatable engineering simulations.

## 3.3 Problems Basilisk solves

A spacecraft is more than an object following an orbit.

Its behaviour can be affected by:
- Its mass and physical structure.
- Its orientation.
- External forces.
- Its reaction wheels.
- Thrusters.
- Sensors.
- Control algorithms.
- Environmental effects.

Engineers need to understand how these systems interact.

Basilisk provides a modular simulation framework to investigate such behaviour.

## 3.4 Main capabilities

### Spacecraft dynamics

Simulate spacecraft translational and rotational motion.

### Six-degree-of-freedom simulation

Model the spacecraft's three-dimensional translation and rotation.

### Attitude dynamics

Investigate spacecraft orientation and attitude-control behaviour.

### Guidance, navigation, and control

Develop and evaluate spacecraft guidance, estimation, and control algorithms.

### Modular system simulation

Connect different spacecraft subsystem models into larger simulations.

### Monte Carlo simulation

Run repeatable simulations with varying input parameters to investigate system behaviour.

### Hardware-in-the-loop

Provide real-time simulation capabilities for hardware-in-the-loop engineering scenarios.

### Flight software development support

Support development and testing of flight-software algorithms in simulation.

### Visualization

Basilisk has a companion visualization application called Vizard.

Vizard uses the Unity rendering engine to display spacecraft states, orientation, orbit, sensors, actuators, and simulation events.

## 3.5 Technical architecture

- Primary user interface: Python.
- Compiled components: C and C++.
- Native components: Rust.
- Interface technology: SWIG for exposing compiled components to Python.
- Visualisation companion: Vizard, based on Unity.
- Licence: ISC Open Source License.
- Platforms: Windows, Linux, and macOS.
- Distribution: Python package with release wheels available through PyPI.

The combination of Python and compiled components provides a balance between configurable simulation scenarios and computational performance.

## 3.6 Who uses Basilisk?

Its documented audiences include:

- Academic researchers.
- Aerospace engineering researchers.
- Space mission analysts.
- Spaceflight algorithm developers.
- Startup space companies.
- Mission developers.
- Engineers investigating spacecraft autonomy.

## 3.7 Limitations and considerations

Basilisk is an engineering framework, not a complete consumer-facing spacecraft application.

Important considerations:

1. Users need knowledge of spacecraft dynamics and simulation.
2. Developing meaningful scenarios requires programming and engineering skills.
3. Users must configure appropriate models and parameters.
4. Simulation results depend on the accuracy of the chosen models.
5. Hardware-in-the-loop simulation does not itself certify flight hardware.
6. A successful simulation does not prove that an actual spacecraft will behave identically.
7. Complex scenarios require careful testing and validation.

These considerations describe the technical demands of the framework, not evidence of defects in Basilisk.

## 3.8 What SpaceJ can learn

- Modular engineering architecture is valuable.
- Physics models should be independently testable.
- Python can make complex engineering systems easier to configure.
- High-performance compiled modules can support computationally intensive simulations.
- Monte Carlo testing is useful for understanding uncertainty.
- Automated verification and validation should be integrated into development.
- Simulation data should be traceable.
- Visualisation can make complex engineering behaviour easier to understand.

## 3.9 Potential opportunities to investigate

These are hypotheses, not validated market gaps.

- Specialised simulation interfaces for particular engineering workflows.
- Better integration between mission analysis and simulation environments.
- Easier experiment configuration and result comparison.
- More accessible engineering data visualisation.
- Specialised analysis and reporting tools.
- Better workflows for selected small-team engineering applications.

Any such product must demonstrate a meaningful advantage over existing tools.

## 3.10 Research conclusion

Basilisk is a powerful modular spacecraft simulation framework.

It provides a significant reference for learning how professional spacecraft simulation systems are structured.

SpaceJ should understand its architecture, experiment with its capabilities, and identify whether specific user workflows remain underserved.

We should not attempt to reproduce its entire simulation framework.

Sources:

https://avslab.github.io/basilisk/

https://github.com/AVSLab

https://github.com/AVSLab/basilisk

Research date: 17 November 2026.

---

# 4. CELESTRAK — SATELLITE ORBITAL DATA INFRASTRUCTURE

## 4.1 Overview

Organisation: CelesTrak.

Official website:
https://celestrak.org/

Official General Perturbations documentation:
https://celestrak.org/NORAD/documentation/gp-data-formats.php

Usage policy:
https://celestrak.org/usage-policy.php

Developer: Dr. T. S. Kelso and the CelesTrak organisation.

## 4.2 What is CelesTrak?

CelesTrak is not an aerospace simulation framework like GMAT or Basilisk.

It is a public space-data resource that provides satellite catalogue information, orbital data, and related space datasets.

Its General Perturbations data service allows developers and researchers to retrieve orbital elements for tracked space objects.

This data can be used by orbital propagation software and other space applications.

## 4.3 What problem does it solve?

Spacecraft and satellites move continuously.

Software systems need orbital information to estimate and visualise their positions and movements.

CelesTrak provides accessible orbital datasets that developers and researchers can retrieve and use in their own applications.

## 4.4 General Perturbations data

CelesTrak provides General Perturbations (GP) orbital data.

These data are derived from observations and are intended for use with the Simplified General Perturbations 4 (SGP4) propagation model.

Historically, developers commonly used Two-Line Element Sets (TLEs).

However, the legacy TLE format has important limitations.

## 4.5 Data formats

CelesTrak supports multiple data formats.

### Legacy formats
- TLE.
- 2LE.
- 3LE.

### Modern OMM-compatible formats
- XML.
- KVN.
- JSON.
- JSON-PRETTY.
- CSV.

These formats provide alternatives to the restrictions of legacy TLE records.

The OMM format is based on the CCSDS Orbit Data Messages standard.

CelesTrak recommends the XML version of OMM Version 2.0 for interoperability.

As of 9 May 2026, CSV is the default response format when FORMAT is not specified.

## 4.6 Important 2026 development

On 11 July 2026, the five-digit satellite catalogue-number limit became an actual issue as newly catalogued objects received six-digit catalogue numbers.

The traditional TLE format cannot represent catalogue numbers above 99999.

This means software depending exclusively on legacy TLE records cannot support all newer catalogue entries.

The OMM-compatible formats provide a path forward.

This is an important example of how changing space-industry requirements can affect software architecture.

## 4.7 Main capabilities

### Satellite identification

Query orbital information using catalogue numbers, names, international designators, and satellite groups.

### Orbital data retrieval

Obtain GP data for supported space objects.

### Multiple formats

Retrieve data in TLE, XML, KVN, JSON, or CSV formats.

### Dataset queries

Retrieve selected objects rather than downloading every available dataset.

### Integration

Use the returned data in other software applications.

## 4.8 Technical architecture and usage

CelesTrak is a data distribution service rather than a single open-source software application.

Developers can retrieve data through HTTP-based queries.

Supported query parameters include:

- CATNR — Satellite catalogue number.
- INTDES — International designator.
- GROUP — Satellite group.
- NAME — Satellite name.
- SPECIAL — Supported special datasets.

Example:

https://celestrak.org/NORAD/elements/gp.php?CATNR=25544&FORMAT=JSON

This requests General Perturbations data for the ISS catalogue number in JSON format.

The underlying data formats follow their respective published specifications.

## 4.9 Who uses CelesTrak?

Potential and documented user communities include:

- Satellite tracking enthusiasts.
- Aerospace researchers.
- Academic institutions.
- Satellite software developers.
- Space mission analysts.
- Organisations developing orbital-data applications.
- Researchers studying orbital behaviour.

## 4.10 Limitations and considerations

1. TLE records cannot represent catalogue numbers above 99999.
2. GP data is intended for SGP4-compatible propagation, not every possible orbital-analysis application.
3. Public orbital data may not be suitable for every precision or safety-critical application.
4. Data can change as updated observations and orbital estimates become available.
5. GP data updates are generally checked by CelesTrak once every two hours.
6. Developers must follow the published usage policy and avoid unnecessary repeated downloads.
7. Network access and data availability must be considered when building dependent applications.
8. CelesTrak data does not replace precise mission-specific navigation or independently verified operational data.

## 4.11 What SpaceJ can learn

- Data infrastructure is an important part of the space industry.
- Public datasets can enable independent engineering research.
- Standardised formats improve interoperability.
- Software must evolve as data standards and catalogue requirements change.
- Applications should support modern formats rather than depend unnecessarily on legacy formats.
- Data caching reduces repeated requests and infrastructure load.
- Data provenance and update timestamps matter.
- Developers must respect the terms and usage limits of external data providers.

## 4.12 Potential opportunities to investigate

These are research hypotheses, not validated market gaps.

- Better tools for processing standardised orbital datasets.
- Improved satellite data visualisation.
- Applications supporting multiple orbital-data formats.
- Dataset validation and provenance tooling.
- Data integration for selected engineering workflows.
- Educational tools for understanding satellite orbital information.

Any potential product must be compared against existing open-source and commercial alternatives.

## 4.13 Research conclusion

CelesTrak provides important satellite orbital data infrastructure.

It is complementary to software such as GMAT and Basilisk.

GMAT and Basilisk can use orbital information in mission and spacecraft analysis workflows, while CelesTrak provides datasets that developers can integrate into applications.

The transition from legacy TLE records to modern OMM-compatible formats is a particularly important engineering consideration.

Sources:

https://celestrak.org/NORAD/documentation/gp-data-formats.php

https://celestrak.org/usage-policy.php

https://celestrak.org/NORAD/documentation/sup-gp-queries.php

Research date: 17 November 2026.

---

# 5. COMPARATIVE ANALYSIS

The three technologies solve different problems.

| Attribute | GMAT | Basilisk | CelesTrak |
|---|---|---|---|
| Category | Mission analysis software | Spacecraft simulation framework | Orbital data service |
| Main purpose | Mission design and navigation | Spacecraft dynamics simulation | Satellite orbital data |
| Main users | Mission analysts and engineers | Simulation and research engineers | Researchers and developers |
| Main technology | C++ with scripting and programming interfaces | Python with C/C++ and Rust components | HTTP queries and standard data formats |
| Open source | Yes | Yes | Public data service; not a software licence |
| Main interface | GUI and scripting | Python programming framework | Web data queries |
| Main strength | Mission analysis | Modular spacecraft simulation | Orbital data accessibility |
| Main challenge for new users | Engineering complexity | Simulation and programming knowledge | Data interpretation and format handling |

## 5.1 How they relate

These technologies can be part of a wider engineering workflow.

A simplified conceptual workflow:

1. Obtain satellite orbital data from CelesTrak.
2. Use an appropriate orbital propagation or mission-analysis tool.
3. Model spacecraft behaviour using a simulation framework such as Basilisk.
4. Analyse the results and compare them with reference data.

This is a conceptual relationship. The exact integration depends on supported formats, models, interfaces, and configuration.

## 5.2 Important distinction

GMAT, Basilisk, and CelesTrak are not direct substitutes for one another.

They serve different purposes:

- GMAT focuses on mission analysis and design.
- Basilisk focuses on spacecraft simulation.
- CelesTrak provides orbital information.

SpaceJ must understand these distinctions before deciding which technical area to enter.

---

# 6. WHAT SPACEJ HAS LEARNED

The initial research provides several important lessons.

## 6.1 Aerospace software is a serious engineering discipline

A spacecraft-related software product may require:

- Mathematics.
- Physics.
- Numerical methods.
- Software engineering.
- Data validation.
- Systems engineering.
- Reproducibility.
- Technical documentation.

A visually impressive application is not automatically an accurate engineering application.

## 6.2 Existing open-source technology is valuable

SpaceJ should not unnecessarily reinvent existing scientific tools.

We should investigate whether existing frameworks can be used, extended, integrated, or complemented.

Before using or adapting any source code, check its exact licence and dependencies.

## 6.3 Data compatibility matters

Legacy file formats can become significant technical obstacles.

Modern applications need to understand evolving standards, data structures, and identifiers.

## 6.4 Simulation must not be confused with reality

A mathematically successful simulation is not proof of a flight-ready spacecraft.

Every simulation needs documented assumptions, appropriate validation, and clearly defined limitations.

## 6.5 Engineering credibility takes time

SpaceJ must demonstrate actual capability through:

- Working software.
- Reproducible results.
- Technical documentation.
- Testing.
- Independent reviews.
- Feedback from knowledgeable users.

---

# 7. POTENTIAL SPACEJ OPPORTUNITIES

The following areas deserve further investigation.

They are not product decisions.

| Research direction | Initial question |
|---|---|
| Mission software | Are there underserved mission-planning workflows? |
| Simulation | Are particular engineering simulations difficult to access? |
| Orbital data | Are there problems integrating and processing different formats? |
| Visualisation | Do engineering teams need more useful ways to inspect results? |
| Ground systems | Which operational workflows consume unnecessary time? |
| Telemetry | Are there unmet analysis or reporting requirements? |
| Education and research | Are there specific tools university aerospace teams lack? |

## Opportunity validation requirements

Before selecting a product, SpaceJ must establish:

1. A specific target user.
2. A genuine recurring problem.
3. Evidence that the problem has meaningful consequences.
4. Existing solutions and their limitations.
5. A technically feasible improvement.
6. A practical way to test the improvement.
7. A potential commercial or strategic benefit.
8. Relevant safety, legal, and data-access requirements.

A promising concept without user evidence remains a hypothesis.

---

# 8. NEXT RESEARCH PHASE

Research-001 is focused on understanding three existing technologies.

The next research phase should investigate actual aerospace workflows.

## Proposed follow-up research

### RESEARCH-002 — Aerospace User Workflow Investigation

Potential participants:
- University satellite teams.
- Aerospace researchers.
- Small satellite engineering organisations.
- Mission analysts.
- Spacecraft software developers.

Questions:
- Which software do they currently use?
- What tasks require the most manual effort?
- Which problems occur repeatedly?
- What software limitations affect their work?
- What tools have they already tried?
- Which problems would justify adopting another product?

### RESEARCH-003 — Existing Product and Market Analysis

Investigate:
- Existing commercial alternatives.
- Open-source alternatives.
- Target users.
- Pricing models.
- Adoption barriers.
- Technical differentiation.
- Possible business models.

### RESEARCH-004 — First Product Selection

Select one engineering problem based on direct evidence and technical feasibility.

Do not select a product simply because it sounds exciting.

---

# 9. RESEARCH SOURCES

Primary sources consulted:

## NASA GMAT

Repository:
https://github.com/NASA/GMAT

NASA Software Catalog:
https://software.nasa.gov/software/GSC-19640-1

Official documentation:
https://gmat.atlassian.net/wiki/spaces/GW/

## Basilisk

Official documentation:
https://avslab.github.io/basilisk/

GitHub:
https://github.com/AVS-Lab/basilisk

## CelesTrak

General Perturbations documentation:
https://celestrak.org/NORAD/documentation/gp-data-formats.php

Usage policy:
https://celestrak.org/usage-policy.php

Supplemental data:
https://celestrak.org/NORAD/documentation/sup-gp-queries.php

## Data standards

Consult the Consultative Committee for Space Data Systems:

https://public.ccsds.org/

The relevant Orbit Data Messages documentation should be reviewed when implementing OMM-compatible systems.

---

# 10. RESEARCH STATUS

Research ID: RESEARCH-001

| Subject | Research status |
|---|---|
| NASA GMAT | Initial research documented |
| Basilisk | Initial research documented |
| CelesTrak | Initial research documented |
| Comparative analysis | Initial analysis documented |
| Opportunity investigation | Not validated |
| User interviews | Pending |
| First product selection | Pending |

## Outstanding work

- [ ] Review GMAT through its documentation and an actual example.
- [ ] Examine Basilisk's architecture and tutorials.
- [ ] Investigate CelesTrak's modern OMM formats.
- [ ] Validate our understanding with practical experiments.
- [ ] Speak to potential aerospace users.
- [ ] Identify recurring engineering problems.
- [ ] Compare potential solutions.
- [ ] Select the first SpaceJ engineering project.

---

# FINAL RESEARCH PRINCIPLE

SpaceJ will not choose its first engineering project based on excitement, appearance, or the ambition of competing with established aerospace companies.

We will study what exists, understand what is missing, identify who needs a solution, and build something technically useful.

Our long-term ambition is to develop aerospace capabilities across launch systems, propulsion, satellites, spacecraft, orbital infrastructure, and exploration.

Our immediate responsibility is to prove that we can solve one real engineering problem.

**Research first. Engineer second. Validate continuously. Expand through evidence.**

---

SPACEJ
India | 2026
