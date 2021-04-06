# MSS (Marine Systems Simulator)

The Marine Systems Simulator (MSS) is a Matlab and Simulink library for marine systems. It includes models for ships, underwater vehicles, unmanned surface vehicles and floating structures. The library also contains guidance, navigation, and control (GNC) blocks for real-time simulation. The algorithms are described in:

    T. I. Fossen (2021). Handbook of Marine Craft Hydrodynamics and Motion Control. 2nd. Edition, Wiley. ISBN-13: 978-1119575054
    Lecture notes: https://www.fossen.biz/wiley
    
which serves as documentation for the toolbox. Please include the following reference when using the MSS libraries: 

    T. I. Fossen and T. Perez (2004). Marine Systems Simulator (MSS)
    URL: https://github.com/cybergalactic/MSS

Copy the contents of the directory MSS/ to your computer and "add the path with subfolders" to Matlab. Then type:

    help MSS

Examples and demo files are located under the catalogs: 

    /MSS/mssExamples/                       Textbook m-file examples (Fossen 2021)  
    /MSS/mssDemos/                          GNC m-file demos
    /MSS/SIMULINK/mssSimulinkDemos/         Simulink demos  
    /MSS/SIMULINK/mssWamitShipXTemplates/   Simulink templates for simulation of WAMIT and ShipX vessel and RAO data
    
The Simulink library (R2021a) is loaded by typing:

    mssSimulink  


 GNC Library
-

Basic libraries and system examples for GNC. The library contains:

- M-file functions (kinematics and kinetics) and examples for time-domain GNC applications.
- M-file library with vessels models, maneuvering trials and dynamic simulation.
- User editable m-files for simulation and control of marine craft including ships, semisubmersibles, autonomous underwater vehicles (AUVs), remotely operated vehicles (ROVs) and unmanned surface vehicles (USVs).
- User editable m-files for error-state Kalman filters for interial navigation systems.

 Hydro Library
-

The toolbox reads output data files generated by hydrodynamic programs and processes the data for use in Matlab. MSS Hydrodynamics includes several example vessels. In order to build your own model, you need a license for one of the following programs:

- 2D strip theory programs - ShipX (Veres) by SINTEF OCEAN AS
- 3D potential theory programs - WAMIT by WAMIT Inc.

The processed data can be used in real-time simulation of marine vessels in 6 DOFs exposed to 1st- and 2nd-order wave loads (motion and force RAO transfer functions) using the Simulink templates located under /MSS/SIMULINK/mssWamitShipXTemplates/.

FDI Toolbox
-
This is a stand-alone toolbox for identification of radiation-force models and fluid-memory effects of marine structures such as marine craft and wave energy converters. Please include the following reference when you use the MSS FDI toolbox:
 
    T. Perez and T. I. Fossen (2009). A Matlab Tool for Parametric Identification of Radiation-Force Models of Ships and Offshore Structures. 
    Modelling, Identification and Control, MIC-30(1):1-15. DOI: https://doi.org/10.4173/mic.2009.1.1 
