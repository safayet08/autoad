# AutoAd
automated ad creation api

```python
Version: 0.0.1     
Authors: Md. Nazmuddoha Ansary 
```
**LOCAL ENVIRONMENT**  
```python
OS          : Ubuntu 18.04.3 LTS (64-bit) Bionic Beaver        
Memory      : 7.7 GiB  
Processor   : Intel® Core™ i5-8250U CPU @ 1.60GHz × 8    
Graphics    : Intel® UHD Graphics 620 (Kabylake GT2)  
Gnome       : 3.28.2  
```
# Setup
* ```pip3 install requirements.txt```

# PoC (Sprint:Exodus)
```python
    EXAMPLE DATA:
    
    data = {'budget'      : 20, # usd
            'start_date'  : '27-1-2021,1:30',
            'end_date'    : '28-1-2021,23:30',
            'objective'   : 'Reach',  
            'channels'    : [{'facebook':{
                            'business_id' :   "760249887886995",
                            'page_id'     :   "Markopoloai",
                            'access_token':   "",
                            'creative_id' :   "23846237956520529",
                            'geo_location': {
                                                'countries':['BD'], 
                                            }
                            }}],

    }
    

```
* The **process_data** under **handler.py** is the entry point for backend data processing (_only facebook for now_)

# NOTES
* **BUDGET**:Must meet a required minimum budget to work (FB POLICY)
* **TODO:** 
    *   Add error handling--> This needs frontend intervention (minor)
    *   launch and test with a creative i.e- change status
* **EXTRACODE**:The **Extra Functions for a/b testing and so-on** section in **fbads.py** are kept for future purposes 




