# Sleep Stage Classification with Accelerometer Data in Apple Watch

## Period
23.07.01 ~ 23.08.31

## Background
수면 중에 잠에서 꺠어나는 상태인 각성이 일어나는 데, 이러한 각성이 자주 일어나는 것은 수면의 질을 떨어뜨리고 여려 질병을 유발할 수 있다.

이러한 문제가 없는지 자신의 수면 단계를 정확하게 파악하는 것은 높은 수면의 질과 건강한 삶을 살기위해 매우 중요하다.

하지만, 기존 뇌파를 통한 수면다원검사 방법(PSG)은 착용이 매우 불편하고 수면 상태를 모니터링하기 위한 전문가가 필요하며, 병원에서만 검사가 가능하다. 

하지만 Apple Watch와 같은 가속 데이터를 활용하면 굳이 병원이 아니더라도 어느 곳에서든지 사용이 가능하며 전문가 없이 스스로 수면 데이터를 얻을 수 있다. 

또한 평소와 같이 수면을 취할 수 있어 정상 수면이 가능하다는 장점이 있다.


## Data
https://physionet.org/content/sleep-accel/1.0.0/

## File
* EDA.ipynb : 각 피험자별 데이터를 EDA한 fille
* Preprocessing.ipynb : 전처리 file
* sleep_df.pkl : 전처리 후 모든 피험자의 데이터를 담은 file
* Modeling.ipynb : 피험자별 수면 분류 모델링 및 결과 file

## Expected Outcomes
기존의 수면 측정 방법보다 더 편리하고 정확한 진단 도구를 개발하는데 기여할 수 있고, 더욱 사용자 친화적인 접근 방식으로 수면 단계를 분석할 수 있고 수면 관련 질환을 파악할 수 있다.

또한, 정확하게 수면 단계를 실시간으로 파악하여 사용자가 원하는 수면 시간 또는 기상 시간을 설정하여 각성 또는 N1 상태를 탐지했을 때 알람을 울리는 기능을 만들어 쾌적한 기상으로 하루를 힘차게 보낼 수 있을 것으로 기대된다.

## Future Work
* Entropy 및 fractal demension 같은 수면 분류에 효과적인 feature를 사용해서 수면 분류 정확도를 더 높일 예정이다.
* Data Augmentation 기법으로 4-class 분류 정확도를 높일 예정이다.


## References
* Olivia Walch, Yitong Huang, Daniel Forger and Cathy Goldstein *Sleep stage prediction with raw acceleration and photoplethysmography heart rate data derived from a consumer wearable device (SLEEPJ , 2019)*
* Andy Stamm, Ronny Hartanto, *Feature Extraction from MEMS Accelerometer and Motion Tracking Measurements in Comparison with Smart Bands during Running (MDPI, 2018)*
* Andy Stamm, David V. Thiel, *Investigating forward velocity and symmetry in freestyle swimming using inertial sensors (Procedia Engineering, 2015)*
