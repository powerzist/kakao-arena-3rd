#### **실행 환경 및 필요 라이브러리**

---

- tags_and_title_tokenize.py
  - 우분투 16.04
  - khaiii 0.4

- inference.py
  - 윈도우 10
  - tqdm 4.47.0
  - scipy 1.5.2

- 공통
  - 파이썬 3.7
  - numpy 1.19.0
  - pandas 1.0.5



#### **실행 순서 및 간략한 코드 설명**

---

1. tags_and_title_tokenize.py
   - data 폴더에 있는 train.json, val.json, test.json 파일에 대해 토큰화 작업 수행
   - data 폴더에 train_with_tt_token.json, val_with_tt_token.json, test_with_tt_token.json 파일 생성
2. inference.py
   - data 폴더에 있는 train_with_tt_token.json, test_with_tt_token.json 파일을 이용하여 예측 수행
   - 예측 결과로 results 폴더에 results.json 파일 생성

- 참고: data 폴더와 results 폴더에 각 코드의 결과 파일들이 이미 생성되어 있습니다.



#### **실행 방법**

---

```sh
python tags_and_title_tokenize.py
```

```sh
python inference.py
```



#### **참고 자료**

---

- [Efficient K-NN for Playlist Continuation](https://eprints.sztaki.hu/9560/1/Kelen_1_30347064_ny.pdf)

- [제목으로 태그 맞추기 with Khaiii, Colab](https://arena.kakao.com/forum/topics/226)

- [Melon Playlist Continuation 대회 데이터 전처리 & EDA](https://arena.kakao.com/forum/topics/191)