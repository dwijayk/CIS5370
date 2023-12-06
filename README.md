# CIS5370
DDOS Attack Detection Using Machine Learning.

we have two different code written in the format of .ipynb (Jupiter notebook)

1- CICDDOS_detection.ipynb

  1-1- make sure that you download the dataset and put that in "DateSets" and save it with name "cicddos2019_dataset.csv"  (you aso can change the path of dataset to any dataset that you want)
  
  1-2- we used "df = df_main.sample(n=100000, random_state=0) " to reduce the training time  (you can add the entire dataset by commenting this line)
  
  1-3- The SMOTHE balancing method is commented out because of the high running time on big dataset
  
  1-4- for jupiter notebook you can run the code section by section or entirely and at the end you will see the result

2- Simulated_dataset_detection.ipynb

  2-1- We have 4 datasets for this part, "DDOS1.csv, DDOS2.csv, benign1.csv, benign2.csv" which we generate the attack using hping3 and
 then capture the datasetusing wireshark and transform it to this format
 
  2-2- the DDOS1.csv and benign1.csv are merged and used for test, DDOS2.csv and benign2.csv are merged and used for training the model.
  
  2-3- a feature mapping is added to allow us to use the same features that we used in CICDDOS_detection.ipynb

