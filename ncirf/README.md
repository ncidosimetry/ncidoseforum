<img width="300" alt="image" src="https://user-images.githubusercontent.com/22055904/233450972-15856234-7bf7-4035-9e56-cdd239c9d07d.png">

# NCIRF3.0

<img width="700" alt="ncirf3 0 20241215" src="https://github.com/user-attachments/assets/34477a43-8d3a-4338-ac36-72685cbbf7f7" />


# [DOWNLOAD LINK](https://nih-my.sharepoint.com/:f:/r/personal/leechoonsik_nih_gov/Documents/ncidoseshare/NCIRF?csf=1&web=1&e=BDRfxZ)
*The download link is accessible exclusively to members with an established Software Transfer Agreement for research use or licensing agreement for commercial use. Please see below for details.

## Available Resources from the download link
- ncirf_batch_input_referencesize.csv
- NCIRF2.0_XXXXXXXX_mac.dmg
- NCIRF2.0.XXXXXXXX_windows.exe
- recommended citation NCIRF2

## Version history
- **20240124 Official release version 2.0.20240124**  
  - Peak Skin Dose now can be calculated through Monte Carlo radiation transport.
  - The new phantom library with the arms rotated was added to more realistically simulate upper extremity x-ray exams.
- 20231116
  - Bug with hardcoded cone beam divergence fixed
  - Arm rotated posture added for upper extremity radiography simulation
- 20230812
  - Errors in Batch Manager-based runs fixed
  - The maximum number of thread increased to 24 
- 20230506
  - MCNP input files can be created from Batch Manager
  - Minor visual errors fixed
- **20221214 Official release version 2.0.20220418**
- 20220418
  - Bug not reflecting custom angles fixed
- 20220317
  - Running on Windows virtual machine on Parallels
  - Error caused by the issues with the path to GEANT4 on non-English Windows fixed
- 20220307
  - Two phantom libraries with the arms raised and lowered are available
  - The initial phantom set to the newborn male phantom
  - Error fixed when no file is selected in “Load Batch Set” on Batch Manager
- 20211217
  - The Mac version with multithreading finally available!
  - Skeletal dose problem discovered in NCIRF1.0 multithread version solved
  - Multithread number can be specified with calculation time (min) displayed
  - No need to install under Documents folder (required for NCIRF1.0)
  - Arm-raised and arm-lowered phantoms available
- **20211206 Official release version 1.0.20211206**
  - Support multithreading for Windows version
  - Bug reported: skeletal doses get zeros
- 20210926
  - Initialize the dose table created from the previous calculation when parameters change
  - Menus for User Manual and User Forum added under “Help” menu
- 20210901
  - Batch manager
  - Users can create a list of parameter sets (patient and technical parameters) by sending them from the GUI to Batch Manager.
  - Users can save/load the list of parameter sets.
  - Users can run the parameter sets in a batch mode
- 20210825
  - Bug not running history greater than 1E7 fixed
- 20210620 Official release version 1.0.20210620
- 20210115
  - NCIRF GEANT4 version completed
  - Critical bugs fixed: half field size, beam angle transformation
- 20200810
  - NCIRF MCNPX version completed
  - Test for Xojo interface to MCNPX input files completed 

## Non-Commercial Research Use

There is no charge to use these resources for non-commercial research purposes. Please click [Software Transfer Agreement form](https://dceg.cancer.gov/tools/radiation-dosimetry-tools/ncidose-software-transfer-agreement.pdf), fill out the form in your web browser*, save it to your computer, then obtain the signatures and submit it to Dr. Choonsik Lee choonsik.lee@nih.gov

## Commercial Use

Contact Dr. Kevin Chang kevin.chang@nih.gov of the NCI Technology Transfer Center to discuss accessing the free trial version and the licensing process for commercial use.
