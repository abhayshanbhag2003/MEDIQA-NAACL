# MEDIQA-NAACL
This repository contains code for MEDIQA 2024 Shared Tasks -> [MEDIQA-CORR: Medical Error Detection & Correction](https://www.codabench.org/competitions/1900/)

## APPROACH
In [finetuning-palmyra-quantised](https://github.com/abhayshanbhag2003/MEDIQA-NAACL/blob/master/finetuning-palmyra-quantised.ipynb), we have first Quantised the Palmyra model to meet the compuational requirments  then fine-tuned it using QLORA which takes input as the text with [MASK] which is done via Gemini then this fine-tuned model replaces the [MASK] with correct disease/vaccine .  

In  [Palmyra-inference](https://github.com/abhayshanbhag2003/MEDIQA-NAACL/blob/master/Palmyra-inference.ipynb), we created a pipeline to create masked texts by identifying the diseases using NER.This disease was then masked with [MASK].This code along with [finetuning-palmyra-quantised](https://github.com/abhayshanbhag2003/MEDIQA-NAACL/blob/master/finetuning-palmyra-quantised.ipynb) helps us identify the error flag along with sentence id and corrected sentence.  

In [RAG_using_Gemini](https://github.com/abhayshanbhag2003/MEDIQA-NAACL/blob/master/RAG_using_Gemini.ipynb) we have implemented our RAG approach to first map the disease/vaaccine from given input text  and then using RAG replace it with correct answer.


### CONTRIBUTORS  
[Sumedh Joshi](https://github.com/sumedhjoshi463)    
[Suramya Jadhav](https://github.com/SURAMYAJ)  
[Atharva Date](https://github.com/Atharva9621)  
[Abhay Shanbhag](https://github.com/abhayshanbhag2003)



