This time we combine our VQA model with voice function.

# Speach To Text(STT) model
The STT model we choose is called Silero Speech-To-Text Models from Silero AI Team.[1] It is a set of compact enterprise-grade pre-trained STT Models for multiple languages. 
Silero Speech-To-Text models provide enterprise grade STT in a compact form-factor for several commonly spoken languages. Unlike conventional ASR models, 
This models are robust to a variety of dialects, codecs, domains, noises, lower sampling rates (for simplicity audio should be resampled to 16 kHz). 
The models consume a normalized audio in the form of samples (i.e. without any pre-processing except for normalization to -1 ... 1) and output frames with token probabilities. 
It provide a decoder utility for simplicity (we could include it into our model itself, but scripted modules had problems with storing model artifacts i.e. labels during certain export scenarios).[1]

![image](https://user-images.githubusercontent.com/90427304/144196531-d8f6258a-b01c-4b5e-a715-18fe7005da96.png)



# Reference
[1] https://colab.research.google.com/github/pytorch/pytorch.github.io/blob/master/assets/hub/snakers4_silero-models_stt.ipynb
