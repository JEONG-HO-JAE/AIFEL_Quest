# AIFFEL Campus Online Code Peer Review 
- 코더 : 정호재
- 리뷰어 : 김태민


# PR(Peer Review)
- [ ]  **1. 주어진 문제를 해결하는 완성된 코드가 제출되었나요?**
    - 문제에서 요구하는 최종 결과물이 첨부되었는지 확인
    - 문제를 해결하는 완성된 코드란 프로젝트 루브릭 3개 중 2개,
        - 1번, 2번은 잘 해결했습니다.
        - 3번은 해결하지 못했습니다. 하지만 해결 할려고하는 모습을 보이시면서 고치실려고 했습니다.
    퀘스트 문제 요구조건 등을 지칭
1. Abstractive 모델 구성을 위한 텍스트 전처리 단계가 체계적으로 진행되었다.
    - 분석 단계
    - 정제 단계
    - ![image](https://github.com/JEONG-HO-JAE/AIFEL_Quest/assets/29370771/79e086fc-10a9-4922-b57c-2f034b5dad69)

    - 정규화와 불용어 제거
    - ![image](https://github.com/JEONG-HO-JAE/AIFEL_Quest/assets/29370771/a6b3e3ea-2934-4508-961e-90f7e00d4e55)
    - ![image](https://github.com/JEONG-HO-JAE/AIFEL_Quest/assets/29370771/f8be6d80-02cd-44ce-a2d9-1013875d6fc6)


    - 데이터셋 분리
    - ![image](https://github.com/JEONG-HO-JAE/AIFEL_Quest/assets/29370771/50e0a2fe-db57-49a8-8e2b-84dedb5d264f)

    - 인코딩 과정
    - ![image](https://github.com/JEONG-HO-JAE/AIFEL_Quest/assets/29370771/34ed5cd3-3638-497f-9f2c-0ca8de65b055)
    - ![image](https://github.com/JEONG-HO-JAE/AIFEL_Quest/assets/29370771/f0873fd4-9937-4a47-b834-d33b04f6d6c4)
    - ![image](https://github.com/JEONG-HO-JAE/AIFEL_Quest/assets/29370771/febc8b4e-7d15-4d26-a64c-733e57d6e479)



2. 텍스트 요약모델이 성공적으로 학습되었음을 확인하였다.
   - ![image](https://github.com/JEONG-HO-JAE/AIFEL_Quest/assets/29370771/4554add1-2d93-44b4-8c7f-33813705f007)

3. Extractive 요약을 시도해 보고 Abstractive 요약 결과와 함께 비교해 보았다.
   - 함께 비교해보았지만 Extractive Summary는 보이지 않는다.
   - ![image](https://github.com/JEONG-HO-JAE/AIFEL_Quest/assets/29370771/af0b0d0a-a82e-44f8-a8d8-2e0fffa7a347)



- [ ]  **2. 전체 코드에서 가장 핵심적이거나 가장 복잡하고 이해하기 어려운 부분에 작성된 
주석 또는 doc string을 보고 해당 코드가 잘 이해되었나요?**
    - 해당 코드 블럭에 doc string/annotation이 달려 있는지 확인

    - 해당 코드가 무슨 기능을 하는지, 왜 그렇게 짜여진건지, 작동 메커니즘이 뭔지 기술.
        - encoder 모델과 decoder 모델의 주석이 잘 작성돼있습니다.
    - ![image](https://github.com/JEONG-HO-JAE/AIFEL_Quest/assets/29370771/43b87b91-d227-4c83-8dcc-f5836840eeb1)
    - ![image](https://github.com/JEONG-HO-JAE/AIFEL_Quest/assets/29370771/c6c2548c-7d50-44d1-8b60-e8b08c7c7210)



        
- [ ]  **3. 에러가 난 부분을 디버깅하여 문제를 “해결한 기록을 남겼거나” 
@@ -23,14 +57,26 @@
    - 문제 원인 및 해결 과정을 잘 기록하였는지 확인
    - 문제에서 요구하는 조건에 더해 추가적으로 수행한 나만의 시도, 실험이 기록되어 있는지 확인
    - 잘 작성되었다고 생각되는 부분을 캡쳐해 근거로 첨부합니다.
        - Extractive summary에 결과가 나오지 않는 부분을 팀원들과 이야기 해보면서 해결해 나갈려고 하는 모습이 있었습니다.
        - 아직 해결이 되지 않았지만, 해결 할 것으로 예상됩니다.
    - ![image](https://github.com/JEONG-HO-JAE/AIFEL_Quest/assets/29370771/8f5b04d0-c907-428c-b8df-b9c0518da661)

        
- [ ]  **4. 회고를 잘 작성했나요?**
    - 주어진 문제를 해결하는 완성된 코드 내지 프로젝트 결과물에 대해 배운점과 아쉬운점, 느낀점 등이 기록되어 있는지 확인
    - 완성된 프로젝트에 대한 평가를 이해쉽게 전체 코드 실행 플로우를 그래프로 그려서 이해를 돕고 있는지 확인
          - 회고를 작성하지 않았습니다.
          - 하지만 주요 요점부분을 작성했습니다.
      - ![image](https://github.com/JEONG-HO-JAE/AIFEL_Quest/assets/29370771/bb986b56-927c-46b8-a125-eeab0cf28705)


- [ ]  **5. 코드가 간결하고 효율적인가요?**
    - 파이썬 스타일 가이드 (PEP8) 를 준수하였는지 확인
          - 잘 준수했습니다.
    - 하드코딩을 하지않고 함수화, 모듈화가 가능한 부분은 함수를 만들거나 클래스로 짰는지 코드 중복을 최소화하고 범용적으로 사용할 수 있도록 함수화했는지
          - preprocessing 부분을 함수화 했습니다.
    - ![image](https://github.com/JEONG-HO-JAE/AIFEL_Quest/assets/29370771/fa44608e-894d-4f3e-bc7f-5d8c61a41cdd)
