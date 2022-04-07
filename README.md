# Pegasus implementation on google colab
The Pegasus model was proposed in PEGASUS: Pre-training with Extracted Gap-sentences for Abstractive Summarization by Jingqing Zhang, Yao Zhao, Mohammad Saleh and Peter J. Liu on Dec 18, 2019. Paper: https://arxiv.org/pdf/1912.08777.pdf

Performing abstractive summarization on a kaggle dataset Link: https://www.kaggle.com/datasets/varunucl/wikihow-summarization?select=wikihowAll.csv

The dataset is a csv file containing 3 columns of headline, title of article and full article.

Initially my idea was to summarize the full article and manually compare the summarized text with title in csv file.

But the model refuses the full article due to large size and even the model was pretrained on max_size_length of 512, 1024 only. So, using the full article would take a lot of time or be inaccurate. Hence I summarized on headline and compared it with the title in csv file.

Due to time constraints I have only used the first 100 data from the csv file.
