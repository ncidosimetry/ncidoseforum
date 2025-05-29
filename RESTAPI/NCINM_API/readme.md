## NCINM API
https://ncinm-xxxxx.xxxxx.xxx/param

*The domain name and cloud server will be configured once the commercial licensing agreement is finalized.

### JSON input

parameter|definition
--|--
|phantom group|1=NCI phantoms, 2=ICRP phantoms|
|gender|1=female,2=male|
|age|patient's age|
|radiopharmaceutical|ID of radiopharmaceuticals 1-137, refer to [ncinm_radiopharmaceuticals.xlsx](ncinm_radiopharmaceuticals.xlsx)|
|activity|administered activity in MBq|

### Example input
[2,1,8,20,200]

parameter|what is means
--|--
|1|ICRP phantom library selected for dose calculations|
|1|patient's gender is female|
|8|patient is 8 years old|
|20|radiopharmaceutical is F-18-fluoro-2-deoxy-D-glucose (FDG) (ICRP 128)|
|200|200 MBq is administered|

### JSON output
organ doses (mGy) for the following target organs/tissues

serial number|target organ name
--|--
|1|Adipose                  
|2|Adrenal                  
|3|Adrenal L                 
|4|Adrenal R                 
|5|Basal cells of bronchi          
|6|Brain                   
|7|Breast adipose              
|8|Breast glandular             
|9|Colon                   
|10|Colon W L                 
|11|Colon W R                 
|12|ET region                 
|13|Gall bladder W              
|14|Gonads                  
|15|Heart W                  
|16|Kidney                  
|17|Kidney C+M+P R             
|18|Kidney C+M+P L             
|19|Kidney cortex L             
|20|Kidney cortex R             
|21|Kidney medulla L             
|22|Kidney medulla R             
|23|Kidney pelvis L             
|24|Kidney pelvis R             
|25|Lenses of eye               
|26|Liver                   
|27|Lung                   
|28|Lung L                  
|29|Lung R                  
|30|Lymph nodes ET
|31|Lymph nodes but ET&Th    
|32|Lymph nodes thoracic      
|33|Muscle                  
|34|Nasal passage Ant
|35|Nasal passage Post+pharynx     
|36|Oesophagus                
|37|Oral mucosa                
|38|Pancreas                 
|39|Pituitary gland              
|40|Prostate or Uterus            
|41|Salivary glands              
|42|Sigmoid+rectum W            
|43|Skin                   
|44|Small intestine W             
|45|Spinal cord                
|46|Spleen                  
|47|Stomach W                 
|48|Thymus                  
|49|Thyroid                  
|50|Tongue                  
|51|Tonsils                  
|52|Ureters                  
|53|Urinary bladder W             
|54|Active Marrow
|55|Shallow Marrow
|56|Effective dose (mSv)|
