## 끝에 특정확장자가 들어가는 파일을 보고싶지 않다면 or commit 제외

.gitignore 파일을 하나 만들어주고 해당 파일에

secret/

*.csv
*.png
*.확장자

를 입력해준다

---

- 개인 프로젝트에 필요하지만 공유되면 안되는 것들.
- 개발환경과 관련된 파일들 
    - ex.운영체제(OS) : windows, 맥(.DS_store)
- 개발 언어 : python
- IDE : 텍스트 에디터

---

## branch

- 원격저장소가 아닌 독립된 저장소
- 독립적인 작업흐름을 만들고 관리

- 순서 : git branch (branch이름) -> git checkout (branch이름)
- git branch (branch 이름) : branch 생성
- git checkout (branch 이름) : 해당 branch로 이동
- 이후 git add (file name) -> git commit -m '(메세지) 해주고 git checkout main -> git push origin main (main 저장소로 이동하여 업로드)

---

## main인 프로젝트에 내가 가져와서 작성 후 다시 올리기

1. main 프로젝트의 주소에 들어가서 'Fork' 클릭하고 Create Fork 클릭
2. 원격저장소에 clone해야함. (반드시 나의 저장소에 클론해주어야 한다.)
    - git clone https://github.com/(나의 원격저장소 주소)/(fork한 name)
    - 명령어는 바탕화면에서 git bash 또는 terminal을 열어서 입력해준다.
    - git 저장소가 아닌 곳에서 (main표기가 없는) 입력해주면 된다.
3. 바탕화면에 fork 받은 폴더가 있는데 이것을 vs code로 열어서 코드 작성 진행.
4. 작성이 끝나면 add, commit, git push origin main 진행
5. Github에 들어가서 Pull Request 만든다.

---

## last 정리
git init은 '프로젝트 초기 세팅하는 사람'만 '프로젝트 시작'때 '딱 한번' 하는 것.
다른사람들은 모두 git clone을 이용해서 clone 받아서 쓰는 것.

2개의 파일중 1개씩 각각 커밋을 하고싶은데 실수로 git add . 을 해버렸다. 돌아가는 방법은?
- ' git restore --staged <file>... ' (add . 할때 돌아가고싶으면 ~~해라 라고 결과창에 적혀있음.)

코드를 다 적어놨는데 시간이 지나서 혹은 실수로 코드가 다 지워졌고 껐다 켜버렸다. 방법은?
- git restore . 입력 (이전 버전으로 되돌려준다.) commit 되어있던 것들은 언제든지 되돌릴 수 있음.

커밋 메세지 변경하는법?
- git commit --amend 
- 버전이 업데이트되기 때문에 내가 push를 한 이후에는 하면 안된다. 
- push를 하는 순간 버전이 달라져서 충돌이 생길 수 있다. push를 하기 전에 미리 변경하자.

