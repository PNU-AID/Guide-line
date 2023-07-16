데이콘 대회 참여방법
==================
## 1. 회원가입
> 데이콘 회원 가입을 진행한다.

## 2. 참여신청
> 관심 있는 대회에 참여 신청을 한다.
> 
> <img width="960" alt="2" src="https://github.com/PNU-AID/Guide-line/assets/95275655/94289439-e8d6-4c6e-9773-bbd62f99a048">

## 3. 데이터 확인
> 데이터 설명을 확인하고 대회 데이터를 다운로드 한다.
> 
> <img width="960" alt="3" src="https://github.com/PNU-AID/Guide-line/assets/95275655/5e7acbd7-19be-49c1-bbe7-978d76de8bad">

## 4. 모델 설계
> 주어진 데이터를 이용해 대회 목적에 맞는 모델을 설계 후 예측 결과 파일을 생성한다.
> 
> '코드 공유' 페이지에 baseline이 있는 경우 이를 참고하면 더 수월하게 문제 해결에 접근할 수 있다.
> 
> <img width="960" alt="4" src="https://github.com/PNU-AID/Guide-line/assets/95275655/50287fa9-9b29-4acb-a887-cf5f2f290a5d">

## 5. 예측 파일 제출
다음으로, 데이콘 홈페이지에서 제출하는 과정이다.

이 과정을 통해 우리의 모델이 목표로 하는 데이터에 대해 어느 정도의 성능을 가지는지, 다른 사람들은 어느 정도의 성능을 얻었는지 확인할 수 있다.

제출에는 두 가지 방법이 있다. API를 이용하여 자동으로 제출되도록 하는 방법과, 직접 csv 파일을 업로드하는 방법이 있다.

### API를 이용하여 제출하기
> https://dacon.io/forum/403557

위의 링크를 참조하여서 개인 토큰을 발급받은 후,

```python
!pip install dacon_submit_api-0.0.4-py3-none-any.whl
```
```python
from dacon_submit_api import dacon_submit_api 

result = dacon_submit_api.post_submission_file(
'파일경로', 
'개인 Token', 
'대회ID', 
'팀이름', 
'submission 메모 내용' )
```

다음과 같은 코드를 이용하여 API를 통해 제출할 수 있다.

### 직접 제출하기
위에서 다양한 분석을 마친 후, 
1. 먼저 대회 페이지에서 제출 탭의 버튼을 누르면 파일 업로드 화면으로 전환된다.

2. 전환된 화면에서 서류모양 아이콘을 클릭하여 제출할 파일을 선택하거나 파일을 마우스로 끌어와 서류모양 아이콘 위에 Drag-Drop 하면 파일을 업로드 할 수 있다.

3. 업로드가 완료되었다면 검은색 제출 버튼을 눌러 제출을 마무리한다.

## 6. 최종 제출
> 리더보드의 Public score를 참고하여 최종 제출 파일을 선정한다.
>
> <img width="960" alt="6" src="https://github.com/PNU-AID/Guide-line/assets/95275655/00f59667-3b42-4086-893b-7d455b117980">
>
> <img width="960" alt="6-2" src="https://github.com/PNU-AID/Guide-line/assets/95275655/5be998e8-5849-4cb7-ae5e-b79e0408a9fd">

코랩으로 데이콘 대회 참여하기
=================
> 링크 : https://dacon.io/competitions/official/235836/talkboard/404882
