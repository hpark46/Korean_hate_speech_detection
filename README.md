# Korean_hate_speech_detection
 
The notebook contains my work on Korean hate speech detection.

Pretrained model used: beomi/KcELECTRA-base

@misc{lee2021kcelectra,
  author = {Junbum Lee},
  title = {KcELECTRA: Korean comments ELECTRA},
  year = {2021},
  publisher = {GitHub},
  journal = {GitHub repository},
  howpublished = {\url{https://github.com/Beomi/KcELECTRA}}
}


Dataset Used: Korean Hate Speech Dataset 
Train Data: labeled train.tsv
Validation Data: dev.tsv
Test Data: test.no_label.tsv 
@ https://github.com/kocohub/korean-hate-speech.git


Dataset: comments, label
comments: str
label: str (none, offensive, hate)


Because the dataset does not provide with a labeled test data,
(and wanted to use all the train/dev data that are provided during the 
training steps)
I used test.no_label.tsv for testing the fine-tuned model. 
https://www.kaggle.com/c/korean-hate-speech-detection/

Submitting the generated prediction, granted with 0.66421 Score
(which I am not sure if the score is solely based on accuracy or calculated 
in some other ways)


Tried to find other labeled dataset for hate speech, but could not find 
a Korean dataset with three labeles (none, offensive, hate)