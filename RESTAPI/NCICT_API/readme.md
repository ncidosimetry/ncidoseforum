## NCICT API
https://ncict-xㅌxxx.xxxxx.com/param

*The domain name and cloud server will be configured once the commercial licensing agreement is finalized.

### JSON input

parameter|definition
--|--
|scan start|scan start location from the top of the head in cm|
|scan end|scan end location from the top of the head in cm|
|phantom group|1-pediatric female,2-pediatric male,3-adult female,4-adult male,5-fetus,6-pregnant woman|
|height|height of patient in cm|
|weight|weight of patient in kg|nance
|tube potential|kVp|
|TCM|tube current modulation strength ranging 0-1|
|CTDI phantom|1-16cm,2-32cm|
|CTDI<sub>vol</sub>|volumetric CT dose index in mGy|

### Example JSON input
[1,10,2,155,50,120,0.5,1,21]

parameter|what is means
--|--
|1|scan starts at 1 cm from the top of the patient's head|
|10|scan ends at 10 cm from the top of the patient's head|
|2|pediatric male phantom group|
|155|patient's height 155 cm|
|55|patient's weight 55 kg|
|120|tube potential of 120 kVp|
|0.5|tube current modulation strength of 0.5|
|1|CTDI<sub>vol</sub> is based on the 16-cm CTDI phantom|
|21|CTDI<sub>vol</sub> of 21 mGy|

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
