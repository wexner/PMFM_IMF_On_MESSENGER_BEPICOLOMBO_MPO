These are the files needed to produce the figures in the paper:
"Determining the Influence of the IMF and Planetary Magnetic Field Models on Mercury's Magnetosphere along Spacecraft Trajectories of MESSENGER, BepiColombo and MPO" by Exner et al. (2024).

In this paper, we employ different planetary magnetic field models (PMFM) for Mercury and model the magnetospheric response to the upstream solar wind's interplanetary magnetic field (IMF) direction.

The PMFMs are representatives for the multitude of available models of Mercury's planetary magnetic field.
The representative models differ in their multipole moment strengths of dipole, quadrupole and octupole.
The used PMFM classes stand for:
    D - largest dipolar value : g10=-216. , g20=-57. , g30=-37.
    Q - largest quadrupolar value : g10=-190. , g20=-75. , g30=-22.
    O - largest octupolar value : g10=-212.8 , g20=-45.2 , g30=-44.3 

The used IMF directions represent commonly encountered IMF directions at Mercury (He et al. (2017) doi: 10.1002/2016JA023687, James et al. (2019) doi: 10.1002/2017JA024435).
The used IMF cases are:
    pnp
    pnp
    npn
    npp  
and indicate the polarity of the IMF Bx, By, and Bz component in the MASO coordinate system.
E.g. pnp stands for 
    IMF Bx = + 14 nT,
    IMF By = -  8 nT,
    IMF Bz = +  6 nT.

The MASO coordinate system (Mercury Anti-Solar Orbital) is a planet-centered system.
The X- component is aligned with the upstream solar wind direction.
The Z- component is antiparallel to the planetary rotation axis.
The Y- compnent completes the right-handed system and points roughly into Mercury's orbital motion.

Under the assumption that aberration angles can be omitted, 
the MASO system is easily converted into the more usual 
system MSO (Mercury Solar Orbital) by switching the 
polarity of the X- and Y- components while leaving the Z- component unchanged.

The trajectories considered in this study are named as follows:
    M1 : MESSENGER's first flyby,
    M2 : MESSENGER's second flyby,
    MSB1 : BepiColombo's first swingby,
    MSB2 : BepiColombo's second swingby,
    MSB3 : BepiColombo's third swingby,
    MSB4 : BepiColombo's fourth swingby,
    MSB6 : BepiColombo's sixth swingby,
    MPO+descendingApoherm
    
The descending apoherm for each MPO orbit is located at $0^\circ$, $45^\circ$, $90^\circ$ and $180^\circ$ with respect to the positive x-axis, i.e., at the nightside, nightside-dawnside, dawnside and dayside, respectively.
The respective trajectory files are named 
    MPO000, MPO045, MPO090, MPO180.


The file names that represent model results by AIKEF are ordered as follows:
trajectory _ Model _ Coordinate System _ PMFM+IMF
E.g. MSB1_AIKEF_MASO_Dnpn stands for
    BepiColombo's first swingby, AIKEF results in the MASO system, PMFM is Dipole, IMF direction is npn
The columns inside the files are named as follows:
    Time	POS_X	POS_Y	POS_Z	B_X	B_Y	B_Z
Where 
    Time in UTC
    POS_X, POS_Y, POS_Z in Kilometer
    B_X, B_Y, B_Z in nT


The file names that represent the theoretical values for the planetary magnetic field models are ordered as follows:
trajectory _ PMFM _ Coordinate System 
E.g. MPO180_classO_MASO stands for
    MPO's orbit with its descending apoherm on the dayside, PMFM is Octupole, in the MASO system
The columns inside the files are named as follows:
    AA	POS_X	POS_Y	POS_Z	B_X	B_Y	B_Z
Where 
    AA in azimuth angle, i.e., the angle between the current orbit point 
    and the orbit's center within the geographic equator plane, 
    counted in the negative mathematical direction. 
    Used in artillery degrees, that is, a full circle is represented by 3600 (three thousand six hundred) degrees.
    POS_X, POS_Y, POS_Z in Kilometer
    B_X, B_Y, B_Z in nT





The hybrid model AIKEF is presented in the following works:
Müller et al. (2011) https://doi.org/10.1016/j.cpc.2010.12.033 
Exner et al. (2018) https://doi.org/10.1016/j.pss.2017.12.016 
Exner et al. (2020) https://doi.org/10.1029/2019JA027691
