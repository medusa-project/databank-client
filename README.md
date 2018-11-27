# databank-client

*Sample API client python script to upload a file to an Illinois Data Bank draft dataset*
https://databank.illinois.edu

Requires recent version of python 2 or 3, works on files up to 2 TB.

**Required Modules**

    pip install tuspy
    pip install requests
    pip install urllib3[secure]

A version of the following usage template command, pre-populated with your dataset identifier and token, comes up in response to clicking on the *Get token for command line tools* button when editing a draft dataset.

      Usage:
          python databank_api_client_v2.py \<DATASET> \<TOKEN> \<FILE> [\<SYSTEM>] 
    
      Upload FILE to an existing draft DATASET created in Illinois Data Bank (https://databank.illinois.edu), authenticating with TOKEN on SYSTEM, which is the production system by default.
    
      Arguments:
        
       DATASET   dataset identifier, unique and persistent within Illinois Data Bank, obtained on screen opened Get token for command line tools button on the edit screen for a draft dataset  
       TOKEN     API authentication token, obtained on screen opened Get Token for Command Line Tools button on the edit screen for a draft dataset   
       FILE      your file to upload
	   SYSTEM    optional system indicator (local | development | production | aws_test), default is production 
    

**What do we mean by a draft dataset?**

A dataset is in a draft state in the Illinois Data Bank after the deposit agreement has been accepted and before the dataset is published or scheduled for publication. Before uploading a file using any of these options, create or find your draft dataset, and navigate to the edit form for that dataset.

**How do I get started?**

At the bottom of the edit screen section for a draft dataset is a matrix of upload options buttons. 
Click the *Get token for command line tools* button to display required elements for use in command line tools.

Notes:

* A token expires in 3 days, but a new one can be requested using the same method.

* Anyone can use a token to upload a file to this dataset, so keep it secure.

* A distinct token is required for each dataset.