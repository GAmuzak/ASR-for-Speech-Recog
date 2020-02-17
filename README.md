# Eva-01
A project to use audio super resolution to upsample english speech and feed to speech recognition softwares for better accuracy

The paper for audio super resolution: https://arxiv.org/pdf/1708.00853.pdf :AUDIO SUPER-RESOLUTION USING NEURAL NETS by Volodymyr Kuleshov, S. Zayd Enam, and Stefano Ermon

The code has been adapted from the following github repo:https://github.com/leekh7411/Fast-Audio-Super-Resolution
All the code has been ported to notebooks for easier runtime accessibility, and uses a modified custom dataset loader for VCTK corpus as provided by kaggle: https://www.kaggle.com/mfekadu/english-multispeaker-corpus-for-voice-cloning/version/1

The code requires the following dependancies:
```
keras==2.3.1
tensorflow==1.15.2
librosa==0.7.2
numpy==1.18.1
scipy==1.4.1
matplotlib==3.1.3
h5py==2.10.0
import_ipynb==0.1.3 #this is only for the connectivity of the jupyter notebooks and importing their modules
```
