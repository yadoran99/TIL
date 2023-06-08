# Q&A

## Q1

commit을 할 때 자주하는게 좋은가 뭉탱이로 올리는게 좋은가?
- 나누어 자주 commit하면 여러 파일 중 일부만 삭제하는것이 가능하다.
- 여러 파일이 있는데 그 중 일부분(또는 하나)의 파일만 삭제할 수 있다.
- 뭉탱이로 commit을 하게되면 일부분(또는 하나)의 파일만을 삭제할 수 없고, 해당 version을 한꺼번에 삭제해야한다.

## Q2

커밋 메세지 작성 방법은?
- 기본적으로 내가 작업한 내용을 잘 담아주면 좋음. (프로젝트때도 마찬가지) ex) 6/7 수업 
- 파일로 할 수 있는 행위는 CRUD (Create, Read, Update, Delete)뿐이라 거의 이러한 내용으로 커밋 메세지를 작성하게 될 것임.

## Q3
파일 여러개 중 일부분만 커밋하는 방법은?
- 전체 파일 중 3개의 파일만 add하고 싶을때 -> git add a.txt b.txt c.txt
- 전체 폴더 중 2개의 폴더만 add하고 싶을때 -> git add a/ b/
- git add . 은 현재 및 하위 디렉토리를 add한다.
- file명에 공백이 있으면 ' '로 묶어서 입력해준다. -> git add 'READ ME.md' (비추)

## Q4

깃헙에 이미지 외에 영상, 피피티는 업로드 못하나요?
- 모든 파일을 관리할 수 있는데 용량 제한이 있다.
- git-lfs 등으로 어느정도 극복을 하나 용량 제한은 유의하자.

## Q5

깃헙 초록색 네모칸을 채우는 방법은 커밋으로만 가능한가요?
- 네. TIL (Today I Learned)를 자주 이용합시다.

## Q6

원격저장소의 이름, Github username을 바꾸면 어떻게 다시 설정하나요?
- 원격저장소 설정을 해줘야한다. 이름, username을 바꾸면 주소도 바뀌기 때문에 기존 원격저장소를 remove 해주고 git remote add origin (주소)로 새로 설정해준다.
---

# 복습질문

## Q1

내가 작업을 완료하고 버전으로 기록하기 위해 실행하는 명령어를 작성해주세요.
- git add <file/directory> -> git commit -m '(message...)'
- git push origin main 은 원격저장소에 보내기 위한 명령어


## Q2

아래의 표현의 의미를 작성하세요.
Untracked
Changes not staged for commit
nothing to commit, working tree clean
- Untracked : 한번도 커밋이 된 적 없는 파일
- nothing to commit, working tree clean : 최근 커밋한 이후로 어떠한 변경사항이 없음

## Q3

Git은 무엇인가?
- 소스코드 버전 관리를 위한 협업 툴

## Q4

Github는 무엇인가?
- Git을 온라인에서 사용할 수 있도록 하는 서비스