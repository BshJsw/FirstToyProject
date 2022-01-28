# FirstToyProject

## 마크다운
마크다운(md file) 작성 가이드 : https://gist.github.com/ihoneymon/652be052a0727ad59601

## 깃 사용 
git clone :
git clone 명령어는 특정 레포지토리에서 최신 버전의 전체 파일을 로컬에 복제합니다. 일반적으로 레포지토리 복제는 최초 한 번만 수행하며, 다시 복제할 필요가 없습니다.
사용 방법은 다음과 같이 사용하며 'git clone' 명령어 뒤에 복제하고자하는 레포지토리 url을 작성합니다.

``` bash
git clone <레포지토리 URL>
```

branch 생성 : 
``` bash
git branch -b <branch name>
```

branch 이동 : 
``` bash
git checkout <branch name>
```

git status:

git clone 명령어로 원격 저장소와 연결이 되었다면, Local에는 다음과 같이 세 가지 영역이 존재합니다.

Working Directory: 현재 작업중인 공간

Staging Area(Index Area): Working Directory에 작업한 파일을 commit 이전에 담는 공간 그리고 git add 명령어로 추가한 파일들이 등록되는 공간

Repository(.git directory): 현재 연결된 git 프로젝트와 관련된 정보를 담고 있는 공간

git status 명령어는 현재 파일의 상태를 확인하는 명령어로 해당 파일이 Staging area에 등록되었는지 그리고 어떤 상태인지 확인할 수 있습니다.

``` bash
git status
```

git add : staging Area로 올림 (git add -A)하면 수정한거 전부 다 올라감

staging area가 있는 이유 : history를 분석하기 위해 개별적으로 commit message를 남기도록 하기 위해서

git pull: 다른 사람이 내용을 변경했다면 develop branch 가 수정되어 있으니, 최신으로 받은 후에 내 브랜치에서 수정된 파일을 합쳐서 올려야 한다.

``` bash
git pull origin <branch name>
```



개발 방법 : 
1. 각자 이름 branch 에서 개발 후 올려 놓고
2. develop 최신으로 받은 후에
3. 합친(merge? rebase?) 후 테스트
4. 배포..할 때 main으로 해야 하는데 아직 잘 몰루
