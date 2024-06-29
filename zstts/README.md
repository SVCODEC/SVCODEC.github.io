<a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc/4.0/80x15.png" /></a> This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/">Creative Commons Attribution-NonCommercial 4.0 International License</a>.

# To facilitate reviewers to uniformly review the relevant supplementary materials, we have added the link to the supplementary materials to this README.md file



## SVCODEC: A Streaming Variable Neural Speech Codec


### Abstract
Based on the SoundStream network framework, this paper proposes a variable bit rate streaming neural speech codec for low bit rate conditions. The codec uses the vector quantised variational auto-encoder (VQ-VAE) algorithm to capture the temporal structure and spectral characteristics of the audio dataset, generates a latent space codebook with a strong correlation with the feature matrix of the target signal, and facilitates the mapping of feature vectors to discrete feature vectors in the latent space to achieve low bit rate compression of speech. In the process of joint quantization training of multiple latent space codebooks using residual vector quantizers (RVQ), an balanced training strategy is introduced to ensure the balanced weight of the codebook, which is convenient for implementing variable bits in the inference process, and multiple comparative experiments are completed by combining the selection and adjustment of the discriminator and loss function. Objective and subjective experimental results show that SVCODEC achieves better reconstructed speech naturalness and higher speech quality than traditional classical speech codecs and existing neural speech codecs, while maintaining the low latency characteristics of the neural speech codec. Therefore, the codec is suitable for low bit rate compressed speech applications. The demo has been publicly released at [[demo](https://svcodec.github.io/)]


## SVCODEC: A Streaming Variable Neural Speech Codec

### datasets
- **LibriSpeech**: The dataset used for training in this paper [[LibriSpeech](https://www.openslr.org/12/) ]
- **LibriTTS**: The dataset used for the contrasting experiments [[LibriTTS](https://www.openslr.org/60/)]
- **LJSpeech**: The dataset used for the contrasting experiments [[LJSpeech](https://keithito.com/LJ-Speech-Dataset/)]
- **Aishell-1**: The dataset used for the contrasting experiments [[Aishell-1](https://www.openslr.org/33/)]


### Pre-training model
1. SVCODEC     checkpoint-1kk-steps   [[SVCODEC](https://drive.google.com/drive/folders/1WXgv7KzsBV2YdydDXuMgEn9xWtNz28Y6?usp=sharing)]
2. SVCODEC v1  checkpoint-1kk-steps [[SVCODEC v1](https://drive.google.com/drive/folders/11OphMT7OVbczW4QAuPJMqsbLxnVt1-_v?usp=sharing)]
3. SVCODEC v2  checkpoint-1kk-steps [[SVCODEC v2](https://drive.google.com/drive/folders/1Lfym_8rR5RwuHoPdso-kcwhemfffrq1t?usp=sharing)]
4. SoundStream checkpoint-1kk-steps [[SoundStream](https://drive.google.com/drive/folders/1ZCaT_jFSavz51yifFKo6cVLmdr1nmxyy?usp=sharing)]

### Experimental results
1. Preliminary Experiments: [Table I] 
- **SVCODEC**: Original experimental metric of SVCODEC  [[SVCODEC](https://drive.google.com/drive/folders/1Vz4ceeRfL5o53YU2SihUU7sdrSF2IguM?usp=sharing)]
- **SVCODEC v1**: Original experimental metric of SVCODEC v1 [[SVCODEC v1](https://drive.google.com/drive/folders/1xmIk9Y-yGdCtiFyGYSNoD7NAQzpfFBUV?usp=sharing)]
- **SVCODEC v2**: Original experimental metric of SVCODEC v2 [[SVCODEC v2](https://drive.google.com/drive/folders/1l232q_rJ8FFrwG2t0jrH15y6M2bgErXC?usp=sharing)]

2. Evaluation of Speech Quality:  [Table II]
- **F0RMSE**: Original experimental data of F0RMSE of multiple codecs[[F0RMSE](https://drive.google.com/drive/folders/1F9jXyWn8ewb9VrLTge5meVjb6Vl26DWl?usp=sharing)]
- **SaRMSE**: Original experimental data of SaRMSE of multiple codecs[[SaRMSE](https://drive.google.com/drive/folders/1lP6CVFSVteOvpKRYW_qIfoqFdhpP6UFx?usp=sharing)]
- **LSD and MCD**: Original experimental data of LSD and MCD of multiple codecs[[LSD and MCD](https://drive.google.com/drive/folders/1GcO6JtHMOwxAVEwEH-M2aSs064FOVQPK?usp=sharing)]

3. Evaluation of Speech Intelligibility:  [Table I, Table III, Fig. 1, Fig.7]
- **ViSQOL**: Original experimental data of ViSQOL of multiple codecs[[ViSQOL](https://drive.google.com/drive/folders/100H0mlDzdWkAQoj6cVCjsiXoP4u0ghyr?usp=sharing)]
- **DNSMOS**: Original experimental data of DNSMOS of multiple codecs[[DNSMOS](https://drive.google.com/drive/folders/16gKwG0oeT3chDCrwXA2HpjcBPIsSDETO?usp=sharing)]
- **PESQ and STOI**: Original experimental data of PESQ and STOI of multiple codecs[[PESQ and STOI](https://drive.google.com/drive/folders/1V0isAoWl5OaVSrtJ1Rji8Q6Gsj7-TZAr?usp=sharing)]

4. Generalization Analysis: [Table V]
- **LibriSpeech**  Original experimental metric of SVCODEC under LibriSpeech [[LibriSpeech](https://drive.google.com/drive/folders/1HT-0lnOkiKXAZO4o1x-at54LNH_dSFCT?usp=sharing)]
- **LibriTTS**  Original experimental metric of SVCODEC under LibriTTS [[LibriTTS](https://drive.google.com/drive/folders/1OjFUgHVGroHy6yvTwiWfJdTkrgmOLHgd?usp=sharing)]
- **LJSpeech**  Original experimental metric of SVCODEC under LJSpeech [[LJSpeech](https://drive.google.com/drive/folders/1WHdROVxaK83rmgTfLVd35cMalTTqgBx5?usp=sharing)]
- **Aishell-1**  Original experimental metric of SVCODEC under Aishell-1 [[Aishell-1](https://drive.google.com/drive/folders/1-RPT9ez40N0jAlqGNVoCkH4sWu0O5DJe?usp=sharing)]


### Experimental demo
- **Listen Online**: [[demo](https://svcodec.github.io/)]