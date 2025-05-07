<img width="300" alt="image" src="https://user-images.githubusercontent.com/22055904/233450972-15856234-7bf7-4035-9e56-cdd239c9d07d.png">

# NCICT2.0

<img width="700" alt="image" src="https://github.com/user-attachments/assets/cc703512-17b8-49f8-92a2-9caa71083e3c" />

## [DOWNLOAD LINK](https://drive.google.com/drive/folders/1B2cI9eewJzRn5DJMaOGJ1RloNv0blxSF?usp=share_link)
*The download link is accessible exclusively to members with an established Software Transfer Agreement for research use or licensing agreement for commercial use.

## Available Resources from the download link
- ncict_batch_input.csv
- NCICT3.0_XXXXXXXX_mac.dmg
- NCICT3.0.XXXXXXXX_windows.exe
- recommended citation NCICT1
- recommended citation NCICT2

## Version history
- 20241216
  - Bug fixed: Batch run menu not working
- **20241215 Official release version 3.0.20241215**
  - Link to the user manual and user forum
- 20240626
  - Bug fixed: X-ray spectrum index switched between 100 and 120 kVp
- 20240229
  - Bug fixed: TCM profile for body phantoms not properly selected 
- 20240125
  - Bug fixed: effective diameter and SSDE not updated when scan range changed
- **20240124 Official release version 3.0.20240124**
  - Head CTDI phantom-based tube current modulation profiles were added to more realistically simulate TCM for pediatric patients.
  - The muscle layer in the frontal and rear views of the phantoms were removed to better visualize the internal anatomy.
- 20230428
  - Frontal and rear views of the ICRP phantoms revised
- **20221214 Official release version 3.0.20221123**
- 20221123
  - NCICT2.0 published: Lee et al. “CT organ dose calculator size adaptive for pediatric and adult patients,” BPEX 8:065020 (2022)
- 20211123
  - Error fixed when a blank line remained in the batch file which is sometimes caused by editing csv file in Excel
- 20211120
  - Tube current profile per image slice is displayed on the left of the phantom picture.
  - “Average CTDI<sub>vol</sub>” is displayed when TCM strength is greater than zero.
  - “Custom CTDI<sub>vol</sub>” is displayed when CTDI<sub>vol</sub> is entered by users..
  - Several bugs related to TCM in the batch module were fixed.
- 20211027
  - Height and weight made uneditable when body size-dependent phantoms selected. The body size is only adjustable using the up and down arrows.
  - Input for pregnant women (phantom group 5) and fetal (phantom group 6) phantoms can be used in batch input
  - Menus for User Manual and User Forum added under “Help” menu
- 20211021
  - mA will be calculated from custom CTDI<sub>vol</sub> values and TCM can be applied to mA
- 20210915
  - Bug stopping the program when the batch input file is not available fixed
  - mA and rotation time separated from mAs to properly adjust mA in the TCM mode
  - mA limit added to limit too high mA for obese patients under TCM mode
  - TCM mode disabled when a custom CTDI<sub>vol</sub> entered
- 20210520
  - NCICT automatically selects a phantom best matching the height and weight of a patient in the batch mode
- **20210513 Official release version 3.0.20210513**
  - A batch function added (see the template input file: ncict_batch_input.csv)
  - Tube current modulation added based on generic modulation profiles
- 20210307
  - Effective diameter for pregnant women phantoms added
- **20200312 Official release version 3.0.20200312**
  - Speed up the scan range dragging on Windows version
- 20191205
  - Mother’s dose added, NCICT 3.0.20191205
  - Presented at RSNA 2019
- 20190301
  - Eight pregnant phantoms with fetus added. Fetal organ dose made available.
  - NCICT3.0 Build 20190301 launched
- **20181118 Official release version 2.0.20181118**
  - 98 more adult phantoms were added to the dose library, completing all 351 phantoms
  - NCICTX presented at AAPM 2018, NCICTX renamed to NCICT 2.0.20181118
- 20160401
  - 72 adult phantoms + 181 pediatric phantoms, NCICTX 20160401
  - NCICTX presented at AAPM 2016
- 20151201
  - NCICT1.0 published in Journal of Radiological Protection: Lee et al. JRP 2015
  - NCICT1.0 presented at RSNA 2015
- **20141201 Official release version 1.0.20141201**
  - ICRP pediatric and adult phantoms replaced NCI phantoms: NCICT 1.0.20141201
- 20120418
  - MATLAB version translated into Visual Basic 6.0 version of NCICT 1.0.20120418
  - Batch routine implemented to automate multiple calculations
  - Public beta testing started with a non-official data agreement form
- 20110517
  - NCI phantom- and MATLAB-based NCICT 1.0.20110517

## Non-Commercial Research Use

There is no charge to use these resources for non-commercial research purposes. Please click [Software Transfer Agreement form](https://dceg.cancer.gov/tools/radiation-dosimetry-tools/ncidose-software-transfer-agreement.pdf), fill out the form in your web browser*, save it to your computer, then obtain the signatures and submit it to Dr. Choonsik Lee choonsik.lee@nih.gov

## Commercial Use

Contact Dr. Kevin Chang kevin.chang@nih.gov of the NCI Technology Transfer Center to discuss accessing the free trial version and the licensing process for commercial use.
