# Git Tutorial

## GitHub 저장소 생성

깃허브에 로그인하고 저장소를 생성한다.  
git-tutorial 이라는 저장소를 생성한다.

## Git Installation

[Git 설치](https://git-scm.com/)  
[소스트리](https://www.sourcetreeapp.com/)

## Git Configuration

git을 설치하면 같이 설치되는 bash 터미널을 연다. 그리고 폴더를 만든다. 

```bash

git clone 저장소주소
cd 저장소이름

```


서명 설정 확인을 위해서 다음 명령어를 사용한다. 

```bash
git config user.name
git config user.email
```

서명 설정을 변경하기 위해서 다음 명령어를 사용한다. 
```bash
git config user.name "Your Name"
git config user.email "Your Email"
``` 
개인용 컴퓨터라면 --global 옵션을 사용한다. 


```bash
git config --global init.defaultBranch main
``` 
PC 주의적 코딩명명법에 의해서 master 브랜치를 main으로 변경한다. 

## Git Basic

리포지터리 폴더에 다음파일을 추가한다.(attendance.yaml)  
```yaml
#출석부
team : wku
members:
  - name: 카리나
    소속 : 에스파
    학번 : 20201234
```

score.yaml 파일을 추가한다. 
```yaml
# 득점 기록

team : wku
logs :
  - name : 카리나
    소속 : 에스파
    학번 : 20201234
    득점 : 3
    사유 : 퀴즈 정답
```

### git status
git status 명령어를 사용해서 파일이 추가되었는지 확인한다. 

tracked 는 파일이 추적되고 있는 상태이다. 즉 한번이라도 깃에 추가된적이 있는 파일이다.  
untracked 는 파일이 추적되고 있지 않은 상태이다. 즉 깃에 추가된적이 없는 파일이다. 

### git add


