
## Week05 내용 정리 

### $git init
- Initialize your repository if you make the first repository.

1. 현재 로컬 git에 추가하고 싶은 디렉토리로 이동 
2. `pwd`  로 위치 확인
3. 위치가 맞다면 `git init` 하여, 로컬 git 초기화

```bash
ls -al //해당 디렉토리 안에 파일 보기 (숨김파일 포함)
ls //해당 디렉토리 안에 파일 보기 
```

### $git clone

### $git config

```bash
git config --global user.email "you@example.com" 
git config --global user.name "Your Name"

git config --global --list 
```

- Git에서 커밋을 할 때 사용하는 email address, user name를 설정

### git 로컬 저장소와 github 외부 저장소 연결 
```bash
git remote add origin ${URL}.git //github에서 만든 repository의 url 주소.git으로 연결
git remote -v //연결되었는지 verify
git push origin main //로컬 -> 외부 저장소로 push
```

### git 외부 저장소에 push 과정
```bash
git pull –rebase origin main -> 외부 저장소에서 pull 해옴 (충돌 방지)
git add .
git commit -m "커밋 메시지"
git push origin main
```
