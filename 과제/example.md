# 과제 - 해설

## branch 생성
- 1번 방법   
일단 `git clone <저장소 url>` 로 저장소를 받아옵니다.  
그리고 `git branch <branch name>` 을 쓰면 branch가 생성됩니다.  
생성된 branch로 `git checkout <branch name>` 을 통해 이동합니다.   
추가하고 싶은 파일을 받아온 저장소 디렉토리에 넣습니다.   
(과제의 경우 LetsDoWeb 이라는 폴더가 컴퓨터 내(보통 c:)에 만들어졌을 겁니다. 거기다 넣으시면 됩니다.)   
다음, `git add <file name>` 을 해줍니다.
파일을 추가해 줬으니 `git commit -m "message"` 커밋을 해줍시다.
이제 push를 해주면 되는데, 본인이 새로 branch를 파고 이걸 그냥 git push하면 아마 에러가 뜰 겁니다.   
`git push origin <branch name>`을 해줍시다. (구글 치면 나와요 ㅠㅠ)

- 2번 방법
branch 생성을 꼭 clone하고 컴퓨터로 받아온 다음 할 필요는 없습니다.  
그 방식이 정석이지만 github에서 지원을 해주죠...   
먼저 아래처럼 branch를 만들고
[image2](./image_assignments/image_ex)

1번을 클릭하고 branch 이름을 적은뒤, 2번에 create branch 누르면 생성이 됩니다.   
새로 만들어진 branch로 clone 해서 가져온 다음, 자신의 컴퓨터에서 작업을 거쳐 푸쉬 해도 되고,   
`git branch -r` 을 통해 원격 저장소의 branch를 확인한 다음 `git checkout -t origin/<branch name>`으로 branch를 받아올 수 있습니다. 이때 checkout에 의해 branch는 자동으로 switch됩니다. (정확히는 같은 이름의 branch에 데이터를 이전하는 것입니다..ㅎ)
이것이 귀찮으면, github에서 새로 만든 branch로 이동하고, 그곳에서 **upload file** 이나 **new file** 을 통해 바로 commit 할 수도 있습니다.  
cmd의 경우 아래 이미지를 참조해 주세요.  
[image3](./image_assignments/image_ex2)
