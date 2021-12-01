This time we combine our VQA model with voice function.

# Speach To Text(STT) model
The STT model we choose is called Silero Speech-To-Text Models from Silero AI Team.[1] It is a set of compact enterprise-grade pre-trained STT Models for multiple languages. 
Silero Speech-To-Text models provide enterprise grade STT in a compact form-factor for several commonly spoken languages. Unlike conventional ASR models, 
This models are robust to a variety of dialects, codecs, domains, noises, lower sampling rates (for simplicity audio should be resampled to 16 kHz). 
The models consume a normalized audio in the form of samples (i.e. without any pre-processing except for normalization to -1 ... 1) and output frames with token probabilities. 
It provide a decoder utility for simplicity.[1]

![image](https://user-images.githubusercontent.com/90427304/144196531-d8f6258a-b01c-4b5e-a715-18fe7005da96.png)



With this STT model, we can record the verbal question about the image using the microphone in our computer. Then tranform the voice file in wav form，which is a standard digital audio file that can record a variety of mono or stereo sound information without distortion. After that, uploading the voice file and run the model. The question will be display in text form.

![image](https://user-images.githubusercontent.com/90427304/144302759-ba12869d-2689-4df7-aa12-a1b9db4a332d.png)

# Reference
[1] https://colab.research.google.com/github/pytorch/pytorch.github.io/blob/master/assets/hub/snakers4_silero-models_stt.ipynb
