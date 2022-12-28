

# CLSTM-SNP: Convolutional neural network to enhance Spiking neural P systems for Named entity recognition based on Long short-term memory network
  A keras implementation of CLSTM-SNP for Named-Entity-Recognition. 

# Dataset
###  conll-2003 and ontonotes5.0

 ## To run the script
Find the keras file under the site-packages corresponding to the python environment and then find the corresponding layers file, replace the recurrent.py file with the recurrent.py file. Then run the python files (cnn+glove+snplstm.py, glove_snplstm.py, snplstm.py) seperately. 
 ```bash
    python3 cnn+glove+snplstm.py
    python3 glove_snplstm.py
    python3 snplstm.py
 ```
 ## Requirements
    0) nltk
    1) numpy
    2) Keras==2.3.1
    3) Tensorflow==1.14 
    4) python=3.6
 

## Inference on trained model

```python
from ner import Parser

p = Parser()

p.load_models("models/")

p.predict("Steve Went to Paris")
##Output [('Steve', 'B-PER'), ('went', 'O'), ('to', 'O'), ('Paris', 'B-LOC')]
```
 
 
 
 
