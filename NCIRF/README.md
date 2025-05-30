<img width="300" alt="image" src="https://user-images.githubusercontent.com/22055904/233450972-15856234-7bf7-4035-9e56-cdd239c9d07d.png">

# NCIRF3.0

<img width="700" alt="ncirf3 0 20241215" src="https://github.com/user-attachments/assets/34477a43-8d3a-4338-ac36-72685cbbf7f7" />

## [DOWNLOAD LINK](https://drive.google.com/drive/folders/1B2cI9eewJzRn5DJMaOGJ1RloNv0blxSF?usp=share_link)
*The download link is accessible exclusively to members with an established Software Transfer Agreement for research use or licensing agreement for commercial use.

## Available Resources from the download link
- ncirf_batch_input_referencesize.csv
- ncirf_batch_input_sizespecific.csv
- NCIRF3.0_XXXXXXXX_mac.dmg
- NCIRF3.0.XXXXXXXX_windows.exe
- recommended citation NCIRF2

## Version history
- 20241217
  - Bug fixed
    - Calculation not working for the first phantom (female 85cm 10kg) in the size-specific library
    - Windows version: packaging issues resolved
    - ncirf_batch_input_sizespecific.csv: thread info missing
- **20241215 Official release version 3.0.20241215**  
  - New features
    - Over 360 pediatric and adult male and female phantoms with various body sizes available for dose calculation
    - Peak skin dose calculation made faster (only 10<sup>5</sup> history required) using dose map smoothing
    - Table thickness input available for explicit Monte Carlo calculations
    - Find the best matching spectrum from Batch Manager
    - Patient age can be used for Batch Manager instead of age group for reference phantoms
    - Link to the user manual and user forum
  - Bug fixed in NCIRF3.0 beta 3.0.20240718
    - X-ray spectrum selection shifted
    - No liver tag in the phantoms 2085015, 1145030, 1175050
    - Double click on Batch Manager doesn't show parameters on GUI
    - Active marrow and endosteum doses for abdominal skeletons slightly smaller 
    - Visualization of the field height wrong for 15-year-old and adult phantoms
- 20240301
  - Bug fixed: field height and width not properly simulated in Geant4
  - Bug fixed: MC particle numbers (generated vs. collimated) not properly implemented 
- 20240208
  - Bug fixed: batch configuration including HVL formatted X.X0 not working
  - Bug fixed: PSD not included in batch output
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
