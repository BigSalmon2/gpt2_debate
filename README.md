# gpt2_debate

This GPT2-devate model generates debate writing text.  
When you enter text at the beginning of the debate writing, the model gives you the rest of the debate writing as long as you want.  

## How to use

This API has 2 routing address

**# POST parameter**

***/long***  
text : begining of the text you want to generate  
number_samples : the number of sentence that will be generated  
length : the length of each sentence  

***/short***  
text : begining of the text you want to generate  
number_samples : the number of word that will be generated  

**# With CLI** :  

curl --location --request POST 'https://main-gpt2-debate-gmlee329.endpoint.ainize.ai/gpt2-debate/long' --form 'text=We have more cases' --form 'num_samples=5' --form 'length=10'
  
curl --location --request POST 'https://main-gpt2-debate-gmlee329.endpoint.ainize.ai/gpt2-debate/short' --form 'text=We have more cases' --form 'num_samples=5'

**# With swagger** : 

You can test this API with swagger.yaml on [swagger editor](https://editor.swagger.io/)
