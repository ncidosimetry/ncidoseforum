## NCIRF API
https://ncirf-xxxxx.xxxxx.xxx/param

*The domain name and cloud server will be configured once the commercial licensing agreement is executed.

### JSON input

parameter|definition
--|--
|phantom group|1=arms raised,2=arms lowered,3=arm rotated|
|age|patient's age in years|
|gender|patient's gender 1=female,2=male|
|energy|x-ray energy in kVp|
|HVL|half value layer in mm|
|SID|source-to-isocenter distance in cm|
|FWidth|field width in cm|
|FHeight|field height in cm|
|DAP|dose area product in Gy-cm<sup>2</sup>|
|PPA|practitioner primary angle in degree|
|PSA|practitioner secondary angle in degree|
|ISOX|isocenter x in cm|
|ISOY|isocenter y in cm|
|ISOZ|isocenter z in cm|
|MC history*|number of history for Monte Carlo simulation|
|threads**|number of threads used for Monte Carlo simulation|

*Theoretically, the more history is used, the longer calculation takes but the more accurate the results are.
recommended history|organs of interest
--|--
10<sup>5</sub>|peak skin dose
10<sup>6</sup>|organs within the beam field
10<sup>7</sup>|organs outside the beam field

**The more threads are used, the faster calculation finishes. The maximum allowable number of threads depends on the capacity of cloud computing server.

### Example input
[2,17,2,50,1.89,80,10,10,100,180,0,12.2,7.2,34.8,500000,2]

parameter|what is means
--|--
|2|phantoms with the arms lowered selected for dose calculations|
|17|Patient is 17 years old|
|2|Patient's gender is female|
|50|x-ray tube potential is 50 kVp|
|1.89|half value layer of x-ray beam is 1.89 mm|
|80|source-to-isocenter distance is 80 cm|
|10|field width is 10 cm|
|10|field height is 10 cm|
|100|DAP is 100 Gy-cm<sup>2</sup>|
|180|Practitioner primary angle is 180 degree|
|0|Practitioner secondary angle is 0 degree|
|12.2|isocenter x is 12.2 cm|
|7.2|isocenter y is 7.2 cm|
|34.8|isocenter z is 34.8|
|2000000|2000000 Monte Carlo history used for dose calculations|
|2|2 threads used for dose calculations|

### JSON output
organ doses (mGy) for the following target organs/tissues

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
|26|Uterus/Prostate|
|27|Ovaries/Testes|
|28|Skin|
|29|Peak Skin Dose|
|30|Muscle|
|31|Active marrow|
|32|Shallow marrow|
|33|Effective dose(mSv)|
