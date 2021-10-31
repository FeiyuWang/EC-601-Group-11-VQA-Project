# Dataset

The dataset used in VQA model is VQA2.0.

Visual Question Answering (VQA) v2.0 is a dataset containing open-ended questions about images. These questions require an understanding of vision, language and commonsense knowledge to answer. It is the second version of the VQA dataset[1].

* 265,016 images (COCO and abstract scenes)
* At least 3 questions (5.4 questions on average) per image
* 10 ground truth answers per question
* 3 plausible (but likely incorrect) answers per question
* Automatic evaluation metric

The most commonly used dataset is VQA2.0

![image](https://user-images.githubusercontent.com/90427304/139571469-3234837c-41ac-4385-8b58-dcaa39bcf122.png)

Single model VQA 2.0 and VizWiz performance in %

![image](https://user-images.githubusercontent.com/90427304/139571528-70a80f46-0fcf-40ae-9843-575e8ff56878.png)

# Model

The model uded in VQA is MMF, MoViE+MCAN model. The MMF uses the same based technologies - Bottom up and top down to analysis imagines and respones with answers by the question raised.[3]

To set the environment, follow the following steps from [4].
* download data
* install dependencies
* Install MMF
* Install maskrcnn-benchmark
* Demo

After the set of environment, input questions and imagines to get the VQA answer result.
```

image_text, question_text = init_widgets(
    #input the URL of imagine, 
    #input the question for the imagine
)
```
Given an exmple of imagine and answer
![image](https://mail.google.com/mail/u/0/?tab=rm&ogbl#inbox?projector=1)
# Reference
[1] https://paperswithcode.com/dataset/visual-question-answering-v2-0

[2] https://arxiv.org/pdf/1904.08920v2.pdf

[3] https://mmf.sh/docs/projects/movie_mcan/

[4] https://colab.research.google.com/drive/1Z9fsh10rFtgWe4uy8nvU4mQmqdokdIRR#scrollTo=HRUp0r_-B9N0
