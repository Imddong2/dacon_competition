# dacon_competition
음성국적분류 경진대회

대회가 처음이라 부족한 것이 많지만 baseline코드 공부하면서 진행해보았습니다.

제공 받은 음성데이터의 데이터 불균형이 심해서 Augmentation을 통해 데이터 수를 늘릴 필요가 있다고 생각했습니다.
소리데이터를 spectrogram으로 변환하면 이미지와 비슷하게 2차원 축으로 설명이 가능하기 때문에 이미지에서 사용되는 Augmentation기법들을 적용시켜 
음성인식에서 큰 효과를 보여줬던 specAugment기법을 음성 국적 분류 모델 학습에 사용해 보았습니다.  
specAugment에서 제안하였던 time masking기법과 frequency masking 기법을 동시에 적용하였습니다. (시간 축과 주파수 축을 랜덤으로 지정하여 0으로 masking)
* specAugment: A Simple Data Augmentation Method for Automatic Speech Recognition(https://arxiv.org/pdf/1904.08779.pdf)

감사합니다.
