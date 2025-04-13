# South-Ostrobothnia-Deep-Seek

This is an experiment to run deep seek large language model fine tuning to improve translation of standard Finnish to South Osthrobothnian dialect. The experiment is based on tutorial https://www.datacamp.com/tutorial/fine-tuning-deepseek-r1-reasoning-model
I ran the experiment with Google Colab with a python notebook. Fine tuning data is done in two passes. Firstly with a bit over 300 standard Finnish and South Osthrobothnian dialect sentence pairs and secondly, on a bit over 2000 standard Finnish and South Osthrobothnia word pair vocabulary. South Osthrobothnian sentences are taken from Pekka Pohjanpää's blog: http://pohopekka.blogspot.com/ 

I'm not sharing the sentence pairs but only standard Finnish that correspond the blog text. The blog text is indexed by the sentence order so that standard Finnish sentences can be matched. I also share the vocabulary. Shared data is placed at directory data/. Note that the blog is Copyrighted material and I haven't reached copyright holder. Therfore I provide only a download function. Use at your own responsibility.

# Usage

Easiest way to run the code is to copy file:
deep_seek_southob_blog.ipynb
to Google Colab and run it there. Choose GPU based resources. If using Google Colab, copy vocabulary and standard Finnish translations data from directory data/ to your Google Drive and set the directories in the beginning of the notebook. Get api keys for hugging and wandb monitoring service. I have placed the keys to Google drive in diretory secrets/, but it may not be the safest approach. You can edit and skip wandb usage if you don't need that. Direcories properly set, the notebook should upload blog and match standard Finnish sentences to the dialect blog. Note that amount of training data is very small. Still the model seems to get some characteristics of South Ostrobothnian dialect.


<img src="https://github.com/user-attachments/assets/168a7010-3738-4f8d-bff1-a3f95e8281ad" width="700" />

