<img width="300" alt="image" src="https://user-images.githubusercontent.com/22055904/233450972-15856234-7bf7-4035-9e56-cdd239c9d07d.png">

<img width="444" alt="Screenshot 2024-12-12 at 5 30 19 PM" src="https://github.com/user-attachments/assets/e875849f-a6cd-4b72-a189-4d9862a95bff" />

## [DOWNLOAD LINK](https://drive.google.com/drive/folders/1B2cI9eewJzRn5DJMaOGJ1RloNv0blxSF?usp=share_link)
*The download link is accessible exclusively to members with an established Software Transfer Agreement for research use or licensing agreement for commercial use.

## Available Resources from the download link
- Phantom Library Naming Convention: III_SSS_AAA_FFF_RRR
  - III: Institution - ICRP, NCI
  - SSS: Size - reference size, body size-specific
  - AAA: Arm posture - arm-attached, armless
  - FFF: Format - binary voxel, dicomrt
  - RRR: Resolution - high resolution (if not indicated), low resolution (lowres)
 
|Institution|Size|Arm Posture|Format|Resolution|
|-----------|----|-----------|------|----------|
|icrp|reference|armless|dicomrt|high|
|nci|bodysize|armless|binary|low|
|nci|pregnant|armless|dicomrt|high|
|nci|reference|arm|binary|high|
|nci|reference|armless|binary|high|
|nci|reference|armless|dicomrt|high|

- #mastertable_nci_reference.xlsx: Master data table for the NCI reference size phantoms
- #mastertable_nci_bodysize.xlsx: Master data table for the NCI body size phantoms

## Version history
- **20241214 Official release**
  - 362 size-specific phantom library voxelized with low resolution added to the repository.
  - ICRP reference pediatric and adult phantoms, UF/NCI pregnant women with fetus phantoms, and UF/NCI reference size phantoms provided in DICOM-RT (DICOM CT and RT STRUCTURE) format
- 20240127
  - 11 phantoms added to the size-specific phantom library (n=362 in total now):
00f051004.3dm
00f065005.3dm
00m051004.3dm
00m065005.3dm
01f065010.3dm
01f075010.3dm
01f095010.3dm
01m065010.3dm
01m075010.3dm
01m095010.3dm
05f115015.3dm
- **20221214 Official release**
- 20220125
  - Ovary location adjusted using Kelsey et al. 2013 measurements in the NCI reference size and size-specific phantom libraries
  - Breast location adjusted using CT images from NWTS in the NCI reference size and size-specific phantom libraries
- 20211208
  - ICRP reference pediatric and adult phantoms in DICOM-RT format available with and without arms
- 20190101
  - Methods to convert the binary format into DICOM-CT and DICOM-structure developed
  - The reference size and body size-dependent libraries were converted.
- 20181113
  - Adjust gamma to 1.0 for the following phantoms:
	05f105020
	05f105025
	05m095020
	30f165050
	30f165100
	30f170080
	30m160055
	30m160060
	30m165080
	30m165085
	30m165090
	30m170055
	30m175055
	30m175060
	30m175070
	30m175075
	30m175085
	30m175090
	30m190075
- 20180907
  - restore muscle hidden: 30m170055
	- arms layer created and arm structures moved to the layer: 30m175090
- 20180906
  - arms separated in 3dm, voxel phantoms (armless) regenerated: 30m160055,30m160060
- 20180419
  - humerus cortical and spongiosa moved to cortical and spongiosa layers, armless phantom revoxelized: 30m175065
- 20180406
  - Significant overlap between ovaries, uterus and colon adjusted: all 10-year females except 10f145XXX
  - spongiosa of 1-year phantoms has two layers: ref_1-year male/female phantoms
- 20180405
  - Separate combined muscle layer: 30m160055
- 20180302
  - missing organs: heart w, kidneys: 30f150045
- 20180208
  - pelvis cortical bone layer fixed for the following phantoms:
	30m175055
	30m175060
	30m175065
	30m175070
	30m175075
- 20170624	pelvis cortical bone layer fixed
	- 30m180075
	- 30m180085
- 20140101
  - Body size-dependent phantom library completed in collaboration with the University of Florida
  - The phantoms available in binary voxel format
- 20100101
  - Reference size pediatric and adult male and female phantoms (n=12) completed
  - The phantoms available in binary voxel format

## Non-Commercial Research Use

There is no charge to use these resources for non-commercial research purposes. Please click [Software Transfer Agreement form](https://dceg.cancer.gov/tools/radiation-dosimetry-tools/ncidose-software-transfer-agreement.pdf), fill out the form in your web browser*, save it to your computer, then obtain the signatures and submit it to Dr. Choonsik Lee choonsik.lee@nih.gov

## Commercial Use

Contact Dr. Kevin Chang kevin.chang@nih.gov of the NCI Technology Transfer Center to discuss accessing the free trial version and the licensing process for commercial use.
