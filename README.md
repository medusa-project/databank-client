# databank-client

*Client python script to upload a file to an Illinois Data Bank draft dataset*

  Illinois Data Bank Upload.

  Usage:
      illinois_data_bank_upload.py [-h] \<FILE> \<DATASET> \<TOKEN> \[\<SYSTEM>\]

  Upload FILE to an existing draft DATASET created in Illinois Data Bank (https://databank.illinois.edu), authenticating with TOKEN on SYSTEM, which is the production system by default.

  Arguments:
    FILE      input file
    DATASET   dataset key, obtained on screen opened by API button on dataset edit screen
    TOKEN     API token, obtained on screen opened by API button on dataset edit screen
    SYSTEM    optional system indicator (local | development | production), default is production

  Options:
    -h --help
