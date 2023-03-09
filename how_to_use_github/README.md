GitHub 사용법
=============
용어 정리
------
이 가이드는 git bash의 설치를 전제합니다.
내 컴퓨터의 파일을 깃허브에 올리기 위해선 원격 저장소(repository)와 로컬 저장소가 필요해요!
깃허브에 파일을 올리는 방법은 다음 세 가지로 구성돼요.
#### 1. 원격 저장소와 로컬 저장소 만들기.
##### 코드 요약
* $ git init
* 원격 저장소(repository)는 깃허브 본인 페이지의 repository 탭에서 new 버튼을 누르면 만들 수 있어요.
<img width="960" alt="1" src="https://user-images.githubusercontent.com/95275655/224065951-038ba5b9-b0c4-4933-b72e-8818baf70f75.png">
<img width="960" alt="2" src="https://user-images.githubusercontent.com/95275655/224066054-a9c49688-d580-4368-b7df-5618d61900cb.png">
<img width="960" alt="3" src="https://user-images.githubusercontent.com/95275655/224066103-f3f5a832-0305-484e-b8b8-97f53901ad38.png">
* 로컬 저장소를 만들기 위해선 업로드하고 싶은 폴더를 마우스 우클릭 해 git bash를 누르고 위의 코드를 입력하면 돼요.
<img width="960" alt="1" src="https://user-images.githubusercontent.com/95275655/224066220-5503b556-79d7-42ec-9ea9-c93a80f0c3dd.png">
<img width="960" alt="2" src="https://user-images.githubusercontent.com/95275655/224066228-82893329-2c5c-4646-9c34-bc30ec44c02c.png">
#### 2. 원격 저장소와 로컬 저장소 연결하기.
##### 코드 요약
* $ git remote add origin 원격저장소 주소
* $ git branch -m master main
* $ git pull origin main
* 깃허브 원격 저장소의 code 버튼을 누르면 주소가 나오는데 이를 copy 해줍니다.
<img width="960" alt="3" src="https://user-images.githubusercontent.com/95275655/224066236-c217d5b7-2b2e-4876-a188-36f825328cd0.png">
* 위의 코드처럼 paste 해줍니다.
* 만약 원격 저장소를 잘못 연결하거나 기존의 연결을 삭제하고 싶다면 아래 명령어를 입력하세요.
* $ git remote rm origin
* 두 저장소의 연결이 완료되었다면 원격 저장소의 기본 branch 이름을 main으로 바꿔줘야 합니다.
* 만약 원격 저장소에 README.md 파일이 있다면 로컬 저장소로 해당 파일을 가져옵니다.(pull)


#### 3. 로컬 저장소의 파일 원격 저장소에 올리기.
##### 코드 요약
* $ git add .
* $ git commit -m "commit message"
* $ git push origin main
* add는 업로드할 파일을 고르는 단계, commit은 해당 파일을 확인하는 단계, 마지막 push는 최종적으로 올리는 단계입니다.
* 만약 특정 파일만 add하고 싶다면 다음 명령어를 입력하면 됩니다.
* $ git add 파일/디렉토리
* "commit message"는 임의로 설정할 수 있습니다.
