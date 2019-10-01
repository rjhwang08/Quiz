```
cd C:\PatternRecognition // c드라이브 PatternRecognition폴더로 이동
git config --global user.name "rjhwang08" // 환경변수 설정을 통해 유저 이름과
git config --global user.email "rjhwang08@gmail.com"  //유저 이메일 등록
git clone https://github.com/rjhwang08/Quiz.git // clone을 통해 깃헙에 Quiz repo를 로컬에 저장 
cd Quiz // PatternRecognition 폴더 안에 생성된 Quiz 폴더로 이동

git add . // Quiz폴더에 저장한 20190924_Quiz1.py  20190930_Quiz2_solution.py 파일을 staging area에 올림
git commit -m "Add 20190924_Quiz1.py & 20190930_Quiz2_solution.py" // 두개의 파일을 커밋
git push // remote repo로 

git branch solution // solution 브랜치 생성
git checkout solution // HEAD가 solution 브랜치를 가리키도록 변경

git add 20190924_Quiz1_solution.py   // staging area에 20190924_Quiz1_solution.py를 올림
git commit -m "Add 20190924_Quiz1_solution.py" // solution 브랜치로 20190924_Quiz1_solution.py를 커밋
git push origin solution // solution 브랜치를 remote repo에 push 함

git checkout master // HEAD가 master 브랜치를 가리키도록 변경
git merge solution // solution 브랜치를 master 브랜치로 merge함(합치기)

git branch -d solution // local solution 브랜치 삭제
git push origin --delete solution // remote solution 브랜치 삭제
```
