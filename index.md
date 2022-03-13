## Real-time End-to-End Korean Menu TTS with Triphone-balanced Corpus

본 논문에서는 메뉴 텍스트에 특화한 한국어 음성합성기를 제안한다. 메뉴에는 외래어가 많아 기존 한국어 음성합성기로는 상용화 가능한 성능을 내지 못하였다. 해당 성능을 높이기 위해 본 연구에서는 외래어, 특히 메뉴 이름에 대한 성능을 높일 수 있는 데이터셋 구축 방안을 연구하였다. 먼저, Triphone 분석을 통해 상대적으로 희소한 음소들의 정보를 잘 반영한 코퍼스를 구성하고 이를 기반으로 학습 데이터셋을 구축하였다. 이후 구축한 데이터셋을 활용하여 현재 공개된 여러가지 TTS 모델을 학습하고 MOS 평가와 RTF 검증을 통해 어떤 모델로 최적화된 실시간 종단간 음성합성 시스템을 만들 수 있는지 실험한다. 본 연구에서 제안한 실시간 종단형 한국어 메뉴 특화 음성합성기는 레스토랑 웨이터 로봇에 포팅하거나, 비대면 서비스 중 하나인 키오스크에 추가되어 사용자의 편의성을 높이는 방향으로 상용화될 수 있다.

In this paper, we present the menu-text-specific Korean TTS system. The names of menu usually are foreign words which is a weak point of the current Korean TTS system. Their performance on is not enough to be generally used. For better performance with foreign words, particularly the menu, we designed the phoneme-balanced dataset. First, we analyze the tri-phone distribution of corpus, and then, constructed corpus that represents relatively rare phonemes well. With this dataset, we trained several open-sourced TTS models. Through MOS and RTF, we evaluate which model is for the optimized real-time end-to-end TTS system. We expect our model can collaborate with a waiter AI robot or non-face-to-face service like a kiosk. With our TTS model, we believe non-face-to-face or robot service can be more user-friendly and human-likely.

### General Speech Samples

| GroundTruth | Generated Speech | Text |
| ----------- | ---------------- | ---- |
|   <audio src="./audiosamples/SGuniverse_09886_gt.wav" type="audio/wav" controls="" preload=""></audio>   |   <audio src="./audiosamples/SGuniverse_09886_confs2.wav" type="audio/wav" controls="" preload=""></audio>               | <embed src="audiosamples/SGuniverse_9886_text.txt" width="400" height="80">  |
| <audio src="./audiosamples/SGuniverse_09918_gt.wav" type="audio/wav" controls="" preload=""></audio>   |   <audio src="./audiosamples/SGuniverse_09918_confs2.wav" type="audio/wav" controls="" preload=""></audio>               | <embed src="audiosamples/SGuniverse_9918_text.txt" width="400" height="80">      |
|        <audio src="./audiosamples/SGuniverse_09946_gt.wav" type="audio/wav" controls="" preload=""></audio>   |   <audio src="./audiosamples/SGuniverse_09946_confs2.wav" type="audio/wav" controls="" preload=""></audio>               | <embed src="audiosamples/SGuniverse_9946_text.txt" width="400" height="80">   |
|         <audio src="./audiosamples/SGuniverse_09954_gt.wav" type="audio/wav" controls="" preload=""></audio>   |   <audio src="./audiosamples/SGuniverse_09954_confs2.wav" type="audio/wav" controls="" preload=""></audio>               | <embed src="audiosamples/SGuniverse_9954_text.txt" width="400" height="80">    |
|         <audio src="./audiosamples/SGuniverse_09992_gt.wav" type="audio/wav" controls="" preload=""></audio>   |   <audio src="./audiosamples/SGuniverse_09992_confs2.wav" type="audio/wav" controls="" preload=""></audio>               | <embed src="audiosamples/SGuniverse_9992_text.txt" width="400" height="80">    |

### Menu Speech Samples 

| GroundTruth | Generated Speech | Text |
| ----------- | ---------------- | ---- |
|         <audio src="./audiosamples/SogangSpeech_22912_gt.wav" type="audio/wav" controls="" preload=""></audio>   |   <audio src="./audiosamples/SogangSpeech_22912_confs2.wav" type="audio/wav" controls="" preload=""></audio>               | <embed src="audiosamples/SogangSpeech_22912_text.txt" width="400" height="80">    |
|         <audio src="./audiosamples/SogangSpeech_22919_gt.wav" type="audio/wav" controls="" preload=""></audio>   |   <audio src="./audiosamples/SogangSpeech_22919_confs2.wav" type="audio/wav" controls="" preload=""></audio>               | <embed src="audiosamples/SogangSpeech_22919_text.txt" width="400" height="80">    |
|         <audio src="./audiosamples/SogangSpeech_22929_gt.wav" type="audio/wav" controls="" preload=""></audio>   |   <audio src="./audiosamples/SogangSpeech_22929_confs2.wav" type="audio/wav" controls="" preload=""></audio>               | <embed src="audiosamples/SogangSpeech_22929_text.txt" width="400" height="80">    |
|         <audio src="./audiosamples/SogangSpeech_22941_gt.wav" type="audio/wav" controls="" preload=""></audio>   |   <audio src="./audiosamples/SogangSpeech_22941_confs2.wav" type="audio/wav" controls="" preload=""></audio>               | <embed src="audiosamples/SogangSpeech_22941_text.txt" width="400" height="80">    |
|         <audio src="./audiosamples/SogangSpeech_22947_gt.wav" type="audio/wav" controls="" preload=""></audio>   |   <audio src="./audiosamples/SogangSpeech_22947_confs2.wav" type="audio/wav" controls="" preload=""></audio>               | <embed src="audiosamples/SogangSpeech_22947_text.txt" width="400" height="80">    |

### Observations

