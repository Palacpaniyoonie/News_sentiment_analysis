# News_sentiment_analysis_recent version
## 경찰청에서 인턴으로 근무하며 내부 프로젝트로 진행한 뉴스 감성분석 모델들입니다. 
## 보안상 분석 데이터 파일은 외부에 공개될 수 없어 코드만 올려놓습니다.
## (데이터라벨링부터 모델 개발까지)프로젝트를 진행하며 한국어 자연어처리에서 가장 중요하다고 생각했던 것은
## 1. 데이터 라벨링 시 라벨링 가이드를 촘촘하게 만들어야 함 2. 토크나이저의 역할이 생각보다 중요하다는 것
## 3. 데이터 리터러시를 기반으로 프로젝트 초기에 빠르게 적합한 모델을 찾아야 함! 
## 프로젝트를 진행하면서 (내부망 분석환경의 문제로) okt, mecab 등 한국어 패키지를 많이 써보지는 못했는데 그 부분이 아쉽네요. 
## 딥러닝 계열 모델들(RNN, CNN 등)은 데이터셋의 규모가 작아 적합하지 않았던 듯 합니다.
## LR 모델의 경우 TF-IDF 방식을 사용하였습니다. (전체 문서에서 많이 등장하는 단어들은 패널티를 주고 특정 문서에서 자주 등장하는 단어들에 가중치를 주는 방식) 
## 조사 등 불용어의 처리가 매우 어려웠는데, TF-IDF 방식으로 하였을 때 자주 등장하는 조사들, 단어들에 패널티가 주어져 다른 모델들에 비해 성능이 우수했던 것 같아요. 
## 느낀점은 이정도로 정리해봅니다.
## 이 코드를 보게 되신다면 피드백 환영입니다.
