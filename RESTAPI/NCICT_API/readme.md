## NCICT API
https://ncict-xxxxx.xxxxx.xxx/param

*The domain name and cloud server will be configured once the commercial licensing agreement is executed.

### JSON input

parameter|definition
--|--
|scan start|scan start location from the top of the head in cm, 10XX landmark ID<sup>1</sup>|
|scan end|scan end location from the top of the head in cm, 10XX landmark ID<sup>1</sup>|
|phantom group|1-pediatric female,2-pediatric male,3-adult female,4-adult male,5-fetus<sup>2</sup>,6-pregnant woman<sup>2</sup>|
|height|height of patient in cm|
|weight|weight of patient in kg|nance
|tube potential|kVp|
|TCM|tube current modulation strength ranging 0-1, custom mA values -1<sup>2</sup>|
|CTDI phantom|1-16cm,2-32cm|
|CTDI<sub>vol</sub>|volumetric CT dose index in mGy|

<sup>1</sup>If you want to define anatomical landmarks instead of location in cm, please enter "Landmark ID" instead as below. The landmark location (cm) will be automatically scaled to a given height of patient.
<sup>2</sup>If users select Phantom Group 5 (fetus) or 6 (pregnant women), the height should be set to 164 (the reference height for an adult female), and the weight should correspond to the gestational age (8, 10, 15, 20, 25, 30, 35, 38 weeks). For example, if users intend to compute the organ doses for a 35-week fetus or a pregnant woman at 20 weeks of pregnancy, they would use the following information: for the fetus, the phantom group is 5, height is 146, and weight is 35; for the pregnant woman, the phantom group is 6, height is 164, and weight is 20.

<img width="343" height="534" alt="image" src="https://github.com/user-attachments/assets/3f387959-bac4-4037-b1dc-d3b15c50c0af"/>

Example usage of landmark ID to define protocols

protocol|scan start landmark ID|scan end landmark ID
--|--|--
|head|1001|1003|
|neck|1002|1005|
|chest|1004|1007|
|abdomen|1006|1008|
|pelvis|1008|1009|
|AP|1006|1009|
|CAP|1004|1009|
|whole body|1001|1010|

<sup>2</sup>If slice-specific mA values from mA modulation are available from DICOM, you can enter an array of mA values after the last parameter, CTDI<sub>vol</sub>. The custom mA values will be automatically populated across the scan range.

### Example JSON input 1: scan start and end locations in cm, TCM strength 0.2
[**1,10**,2,155,50,120,0.2,1,21]

parameter|what is means
--|--
|**1**|**scan starts at 1 cm from the top of the patient's head**|
|**10**|**scan ends at 10 cm from the top of the patient's head**|
|2|pediatric male phantom group|
|155|patient's height 155 cm|
|55|patient's weight 55 kg|
|120|tube potential of 120 kVp|
|**0.2**|**tube current modulation strength of 0.2**|
|1|CTDI<sub>vol</sub> is based on the 16-cm CTDI phantom|
|21|CTDI<sub>vol</sub> of 21 mGy|

### Example JSON input 2: scan start and end landmark IDs, TCM strength 0.2
[**1006,1009**,2,155,50,120,0.2,1,21]

parameter|what is means
--|--
|**1006**|**scan starts at the bottom of diaphragm**|
|**1009**|**scan ends at pubic symphasis**|
|2|pediatric male phantom group|
|155|patient's height 155 cm|
|55|patient's weight 55 kg|
|120|tube potential of 120 kVp|
|**0.2**|**tube current modulation strength of 0.2**|
|1|CTDI<sub>vol</sub> is based on the 16-cm CTDI phantom|
|21|CTDI<sub>vol</sub> of 21 mGy|

### Example JSON input 3: scan start and end landmark IDs, custom mA values
[**1006,1009**,2,155,50,120,**-1**,1,21,**23,23,23,23,26,29,32,42,51,57,63,71,71,71,71,66,63,60,58,56**]

parameter|what is means
--|--
|1006|scan starts at the bottom of diaphragm|
|1009|scan ends at pubic symphasis|
|2|pediatric male phantom group|
|155|patient's height 155 cm|
|55|patient's weight 55 kg|
|120|tube potential of 120 kVp|
|**-1**|**custom mA values available**|
|1|CTDI<sub>vol</sub> is based on the 16-cm CTDI phantom|
|21|CTDI<sub>vol</sub> of 21 mGy|
|**23,23,23,23,26,29,32,42,51,57,63,71,71,71,71,66,63,60,58,56**|**custom mA**|

### JSON output
organ doses (mGy) for the following organs

serial number|organ name
--|--
|1|Brain|
|2|Pituitary gland|
|3|Lens|
|4|Eye balls|
|5|Salivary glands|
|6|Oral cavity|
|7|Spinal cord|
|8|Thyroid|
|9|Esophagus|
|10|Trachea|
|11|Thymus|
|12|Lungs|
|13|Breast|
|14|Heart wall|
|15|Stomach wall|
|16|Liver|
|17|Gall bladder|
|18|Adrenals|
|19|Spleen|
|20|Pancreas|
|21|Kidney|
|22|Small intestine|
|23|Colon|
|24|Rectosigmoid|
|25|Urinary bladder|
|26|Prostate|
|27|Uterus|
|28|Testes|
|29|Ovaries|
|30|Skin|
|31|Muscle|
|32|Active marrow|
|33|Shallow marrow|
|34|Effective dose (mSv)|
