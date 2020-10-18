# Dermatologist AI To Detect Skin Cancer
Skin Cancer is the most common cancer in the world. In U.S., there are 5.4 million new cases every year. They come in different types. Some are called Carcinomas and some are called Melanomas. Melanomas are the ones that typically kill people, its called the Black Cancer. 20% of Americans eventually get skin cancer. In most cases benign. Pre-cancer also called Actinic Kertosis, affects 58 miliion Americans and many more in the world. In this country there are 76,000 Melanomas each year and 10,000 deaths. Skin cancers comes in multiple stages from stage zero to stage four. 

According to the American Cancer Society, the 5-year survival rate for stage 4 melanoma is 15–20 percent. This means that an estimated 15–20 percent of people with stage 4 melanoma will be alive 5 years after diagnosis. But the 5-year survival rate for Stage 0, is 98.4%. Therefore the early detection is paramount to not dying from skin cancer.

Dermatologists are extremely highly trained to find melanomas and carcinomas, because they need to make life and death decisions in diagnosing patient's skin. But they are very few in numbers and the early detection is still a problem. If human intelligence is also aided with an highly trained AI deep neural networks, it can revolutionize and save the world, by early detection.

## Goal
Skin cancer is primarily diagnosed visually, beginning with an initial clinical screening and followed potentially by dermoscopic analysis, a biopsy and histopathological examination. Automated classification of skin lesions using images is a challenging task owing to the fine-grained variability in the appearance of skin lesions. Deep convolutional neural networks (CNNs) show potential for general and highly variable tasks across many fine-grained object categories [[ 1 ] ](https://www.nature.com/articles/nature21056.epdf?author_access_token=8oxIcYWf5UNrNpHsUHd2StRgN0jAjWel9jnR3ZoTv0NXpMHRAJy8Qn10ys2O4tuPakXos4UhQAFZ750CsBNMMsISFHIKinKDMKjShCpHIlYPYUHhNzkn6pSnOCt0Ftf6)

The goal of this project is to design an algorithm that can visually diagnose melanoma. In particular, the algorithm will distinguish this malignant skin tumor from two types of benign lesions (nevi and seborrheic keratoses).

## Model
Inception v3 using PyTorch as Framework.

## Evaluation
The model is ranked according to three separate categories:

### Category 1 (Score 1): ROC AUC for melanoma classification.
This is the ability to distiguish between malignant melanoma and the benign skin lesions (nevus, seborrheic keratosis) by calculating the area under the receiver operating characteristic curve (ROC AUC) corresponding to this binary classification task.

### Category 2 (Score 2): ROC AUC for melanocytic classification:
All of the skin lesions that we will examine are caused by abnormal growth of either melanocytes or keratinocytes, which are two different types of epidermal skin cells. Melanomas and nevi are derived from melanocytes, whereas seborrheic keratoses are derived from keratinocytes. The second caterory tests the ability to distinguish between melanocytic and keratinocytic skin lesions.

### Category 3 (Score 3): Mean ROC AUC:
This catefory take the average of the ROC AUC values from the first two categories.

## Result
Work under progress
