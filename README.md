
<img width="1743" height="869" alt="038d84d5972aa57ab4767518e32ffcdc" src="https://github.com/user-attachments/assets/f7c8c1b2-2c39-49e2-b1aa-08f78e3f1932" />


Program Introduction

Across these three, studio-style courses—Physical Oceanography, Remote Oceanography, and Time-Series Analysis—students learn to turn raw observations and model output into scientific insight. We work hands-on with real datasets (moorings, drifters, satellites, reanalyses, biogeochemical models), emphasizing reproducible workflows in Python (and optional Julia). Core skills include frequency-domain thinking, spectral and wavelet methods, satellite data processing, and numerical simulation of ocean circulation and tracers. By the end, students can diagnose key ocean processes—from winds driving near-inertial currents to mesoscale eddies modulating biology—and communicate results with publication-quality figures and concise, quantitative writing.

What you’ll do (highlights):

Build and quality-control time series; analyze in the frequency domain (FFT, rotary spectra, coherence) and the time–frequency domain (wavelets).

Process satellite L3/L4 products (e.g., SST, chlorophyll, altimetry) and collocate with in-situ moorings or drifters.

Run and evaluate simple numerical experiments (slab-ocean inertial response, 1-D mixed-layer heat budget, passive-tracer and NPZD-style biogeochemistry).

Reproduce mini case studies (coastal upwelling pulses, diurnal warming, storm-forced near-inertial oscillations, eddy–biology interactions).

Tools & data: Python (xarray, numpy, pandas, matplotlib, cartopy, pywavelets), Jupyter, Git; datasets such as HYCOM/Mercator, ERA5 winds, satellite SST/OC/SSH, coastal moorings and drifters.
Assessment: short practicals (weekly), two mini-projects, one integrative final project with an open-data repo.

Course 1: Physical Oceanography (Process-based foundations)

This course builds physical intuition for the upper ocean. We connect governing equations to observable signals: Ekman layers and wind work, geostrophy and pressure gradients, mixed-layer dynamics, internal waves and near-inertial motions, mesoscale eddies, and boundary currents. Labs couple simple theory with data: estimate geostrophic currents from SSH, compute wind stress and Ekman transport, diagnose a mixed-layer heat budget, and simulate a slab-ocean forced by a wind pulse to capture the anticlockwise inertial response at mid-latitudes.

Example practicals:

Storm event analysis: wind work → near-inertial KE (spectra & rotary decomposition).

Mixed-layer entrainment during upwelling relaxation (comparing mooring T/S to reanalysis fluxes).

Course 2: Remote Oceanography (Satellites, mapping, and synthesis)

We learn end-to-end satellite analysis: choosing products, subsetting, gridding, and bias-checking with in-situ data. Topics include SST and chlorophyll retrievals, sea-level anomaly and geostrophic velocity, ocean color algorithms, and multi-sensor fusion. Students build regional composites, track eddies, and quantify frontal/filament activity, then interpret physical–biogeochemical coupling.

Example practicals:

Eddy census from altimetry: eddy kinetic energy and chlorophyll anomalies relative to eddy centers.

Coastal filament mapping: SST/chl fronts, alongshore wind forcing, and surface current proxies.

Course 3: Time-Series Analysis (From raw signals to mechanisms)

This course is the quantitative backbone: sampling theory, detrending, gap filling, spectra (FFT, Welch, multitaper), rotary and cross-spectra, coherence/phase, band-pass filtering, and wavelet analysis for non-stationary signals. We emphasize uncertainty and significance testing. Students apply these tools to moorings and model output to separate diurnal/semidiurnal tides, inertial bands, and lower-frequency variability, then link diagnostics to dynamics.

Example practicals:

Wavelet power of near-surface currents: time–frequency tracking of inertial bursts after wind events.

Cross-spectral analysis of wind vs. surface currents to quantify frequency-dependent coupling.

Learning Outcomes

By completing the sequence, students will be able to:

Explain and diagnose key upper-ocean processes using observations, theory, and simple models.

Process satellite and in-situ datasets, perform rigorous spectral/wavelet analyses, and evaluate significance.

Design, run, and interpret targeted numerical experiments (physical and simple biogeochemical).

Communicate clearly with figures, notebooks, and concise writing; publish a clean, reproducible project repo.

If you want, I can tailor the examples and datasets to your region (e.g., central Chile, ~36°S) and include a week-by-week outline with readings and graded rubrics.
