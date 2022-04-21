new api for determine / categorize words or sentences
you can customize the category ( negative, positive, neutral )
the machine learning also using sentimental analysis processing including 
learning to new words from input for faster results in next process.

usage : 

call the machineword->analyze('KEYWORDS',1/0 ( training mode ), 'custom_key for batch process') from controllers
note :
first param : the keywords or sentences that needs to be checked
second param : the flag for faster results but less accuracy, default 1
third param : custom key for generating different training results and differ process for batch checking


1. change configurations in libraries/machinewords.php $this->registered of line 21 into your desired category
2. change keywords file in folder libraries/keyword/. note : don't change the supportive.json and the training.json file are mandatory.
3. if you don't have data or list of category please leave it as blank file
4. if you want batch process