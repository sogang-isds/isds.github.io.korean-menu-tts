## A Korean TTS system using Conformer-based FastSpeech2

본 논문에서는 콘포머 기반 FastSpeech2를 이용한 한국어 메뉴 음성합성기를 제안한다. 콘포머는 본래 음성인식 분야에서 제안된 구조로, 합성곱 신경망과 트랜스포머를 결합하여 광역과 지역 정보를 모두 잘 추출할 수 있도록 한 구조다. 이를 위해 순방향 신경방를 반으로 나누어 제일 처음과 마지막에 위치시켜 멀티 헤드 셀프 어텐션 모듈과 합성곱 신경망을 감싸는 마카론 구조를 구성했다. 본 연구에서는 한국어 음성인식에서 좋은 성능이 확인된 콘포머 구조를 한국어 음성합성에 도입하였다. 기존 음성합성 모델과의 비교를 위하여 트랜스포머 기반의 FastSpeech2와 콘포머 기반의 FastSpeech2를 학습하였다. 이때 데이터셋은 음소 분포를 고려한 자체 제작 데이터셋을 이용하였다. ParallelWave GAN을 이용하여 합성음을 생성하고, 평가한 결과 콘포머 기반의 FastSpeech2가 월등한 성능인 MOS 4.06을 달성했다. 본 연구를 통해 한국어 음성합성 모델에서, 동일한 구조를 트랜스포머에서 콘포머로 변경하였을 때 성능이 개선됨을 확인하였다. 

In this paper, we present the korean-menu-TTS system using conformer-based FastSpeech2. Conformer is the convolution-augmented transformer, which was originally proposed in Speech Recognition. Combining two different structures, the Conformer extracts better both local and global features. It comprises two half Feed Forward module at the front and the end, sandwiching the Multi-Head Self-Attention module and Convolution module. We introduce the Conformer in Korean TTS, as we know it works well in Korean Speech Recognition. For comparison between transformer-based TTS model and Conformer-based one, we train FastSpeech2 and Conformer-based FastSpeech2. We collected a phoneme-balanced dataset and used this for training our models. As a result of generating a synthesized sound using ParallelWave Gan, the Conformer-based FastSpeech2 achieved superior performance of MOS 4.06. We confirm that the model performance improved when the same structure was changed from transformer to Conformer in the Korean TTS.

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

