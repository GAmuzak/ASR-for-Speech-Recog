1. Create virtualenv:
   virtualenv -p python3 $HOME/tmp/deepspeech-venv/
   
2. Activate virtualenv
   source $HOME/tmp/deepspeech-venv/bin/activate

3. You first need to git clone the DeepSpeech repository , Install DeepSpeech:
   $pip3 install deepspeech  
   $pip3 install --upgrade deepspeech  

4. Download pre-trained English model and extract by one of the following two methods:
   curl -LO https://github.com/mozilla/DeepSpeech/releases/download/v0.6.1/deepspeech-0.6.1-models.tar.gz
   tar xvf deepspeech-0.6.1-models.tar.gz
   
   OR
   
   wget https://github.com/mozilla/DeepSpeech/releases/download/v0.6.1/deepspeech-0.6.1-models.tar.gz
   tar xvf deepspeech-0.6.1-models.tar.gz

5. Move the deepspeech-0.6.1-models folder into DeepSpeech folder. Create a folder "audio" and store .wav audio file in it.

6. Transcribe an audio file:
   deepspeech --model deepspeech-0.6.1-models/output_graph.pbmm --lm deepspeech-0.6.1-models/lm.binary --trie deepspeech-0.6.1-models/trie --audio audio/2830-3980-0043.wav
