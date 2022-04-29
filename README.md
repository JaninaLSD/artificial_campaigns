# A fine-tuned GPT-Neo model for tweet generation 

## The model 

You can find our model in the folder `gpt-neo-1.3B-user-v1`. This model is a fine-tuned version of the 1.3B-parameter GPT-Neo model by EleutherAI. 

As the default GPT-Neo model did not receive any social media data during its pre-training, we fine-tuned it with tweets collected from Twitter from October to November 2021 related to climate change hashtags. The model received data in the format `<username> - <tweet>` We used an 80/20 train/test split, and to differentiate distinct tweets, we added a start-of-tweet and an end-of-tweet token to the training dataset.
	
To guide you using this model, please consult the `Code/gpt_neo_1.3B_twitter.ipynb` Jupyter Notebook file. 

## The data 

You can find the original tweets we collected from October, 01 to November 07, 2021, in the folder `Data/Original Tweet Ids`. The campaigns including the GPT-generated tweets we used in our publication can be found in `Data/GPT-generated Tweets`. Here, also a file with some original tweets of each user used as blueprint by GPT can be found. Please note that to prevent implications on individuals or organizations implicitly mentioned in the textual data, we pseudonymized the tweets. 


## Reference 

Please cite the following paper if you are uisng this model or data: 

```
@inproceedings{pohl_2022_artificial,
  author       = {Pohl, Janina Susanne and
                  Assenmacher, Dennis and
                  Seiler, Moritz Vincent and
                  Trautmann, Heike and
                  Grimme, Christian},
  title        = {{Artificial Social Media Campaign Creation for Benchmarking and Challenging Detection Approaches}},
  year         = {2022},
  booktitle	   = {{Proceedings of the 16$^{th}$ International Conference on Web and Social Media}},
  series 	   = {ICWSM'22},
  publisher    = {Association for the Advancement of Artificial Intelligence (AAI)},
  address      = {Hybrid: Atlanta, Georgia, US and Online}, 
  numpages 	   = {10}
} 
```

---
license: cc-by-sa-3.0
---
