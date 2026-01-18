```
# 1. 기존 가상환경 종료
deactivate

# 2. 홈 디렉터리로 이동 후 git clone
cd ~
git clone https://github.com/checkCJY/boooooom.git

# 3. 디렉터리 생성 확인
ls -l
-> boooooom 폴더 생성 확인

# 4. 디렉토리 이동후 vscode 재시작
cd boooooom
pwd
-> 경로 확인해주세요. /home/"여러분이름"/boooooom
code -r .
-> 현재 vscode 를 boooooom 디렉토리에서 재시작

# 4.1 해당 디렉토리에서 git 연결 확인
git remote -v 
-> 해당 명령어 입력 후 아무것도 안뜹니다.
-> 뜬다면 주소를 확인해보세요. 2가지 경우의 수 입니다
  1. 가상환경이 안꺼진 상태거나, 상위 디렉토리에 .git이 있어서 잡혀있는 경우
  2. 제 예상과 다르게 이미 접속하고자 하는 repo에 접속이 된경우
    -> 이 경우 repo 주소에 boooooom 이 포함된 주소일 것 입니다.

# 5. uv를 이용한 깃초기화(생략), uv 가상환경 만들기
> 생략하는 이유는 pyproject.toml 파일이 있기 때문입니다.
uv venv

# 6. 가상환경 실행 및 pip설치
source .venv/bin/activate
uv pip install -r requirements.txt

# 7. 원격저장소 설정 
git branch -M main
-> git local branch를 main으로 잡겠다.

# 8. 원격저장소 설정
git remote -v 
-> 내용이 나온다면 아래내용 생략. 이미 연결된상태

git remote add origin 프로젝트 주소

# github 관련 간단 명령어 사용예시와 내용
https://holjjack.tistory.com/212
https://despiteallthat.tistory.com/273

# git 간단한 명령어 실습주소.
[https://learngitbranching.js.org/?locale=ko]
```
