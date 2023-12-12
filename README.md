# Dreambooth
 Implementation of Dreambooth to generate your photorealistic images
<p float="left">
  <img src="images/generated_image8.png" width="300"/>
  <img src="images/generated_image9.png" width="300"/>
</p>

## Installation
It makes use of the Auotrain-advanced package from hugging face: https://github.com/huggingface/autotrain-advanced. Please note you will need python >= 3.8 for AutoTrain Advanced to work properly.
```
pip install autotrain-advanced
```
## How to run
Make a folder called 'images' after cloning the repo in the repository. Add 5-6 images that you want to fine-tune the model.
```
python AutoTrain_Dreambooth.py
```
The above line will create a folder called 'my_dreambooth_project' to store the weights of the model.
Moreover, the output images will be stored as generated_image.

Ideally, the prompt should include a unique code identifier such as 'sks person', 'sks dog', so the model doesn't get confused with existing names. 

Will take around 45 mins for a single cycle of generation on a local machine. Tested on Nvidia 2080 card.
