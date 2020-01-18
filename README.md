### Installation
The module, topis requires pandas, math and sys modules to function
This module is used to print the score and rank after using TOPSIS (Technique for Order Preference based on Similarity to Ideal Solution)
```sh
$ pip install topsis
$ python
>> import topsis
>> top_obj = topsis.Topsis('data.csv') # input file is data.csv with all numberical data
>> print(top_obj.d) # prints the normalized matrix
>> print(top_obj.features) # prints number of features(columns)
>> print(top_obj.samples) # prints number of tuples or samples(rows)
>> top_obj.evaluate(w=[1,1,1],im=["+","+","-"]) #since data.csv has 3 features with last to be minimized and first two maximized
''' w is the weight list and im is the impact list where "+" is used for maximize and "-" for minimize. Size of w, im is equal to number of features. Default weight is 1 and impact is "+" '''
```
### License
MIT
### Author
Sahil Ahuja
