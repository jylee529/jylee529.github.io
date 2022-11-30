
# 내가 프로젝트를 build한 과정

## 1. 지킬 설치
- 루비 인스톨러 홈페이지에서 Ruby+Devkit 3.1.3-1 (x64) 을 다운로드 했다.
- 그 다음 ruby 콘솔을 실행하여 다음 명령어를 입력했다.
```yml
gem install jekyll
gem install minima
gem install bundler
gem install jekyll-feed
gem install tzinfo-data
```
- 이제 깃허브 리퍼지터리에서 jylee529.github.io라는 이름의 리퍼지터리를 만들었다.
- 그 리퍼지터리에서 링크를 복사하고 터미널에서 다음 명령어를 입력했다.
```yml
git clone https://github.com/jylee529/jylee529.github.io.git
```
- 이제 생성된 디렉터리에 cd로 접근하고 다음 명령어로 지킬 기본 파일을 생성했다.
```yml
jekyll new . --force
```
- 아래 명령어로 지킬 서버를 실행했다.
```yml
jekyll exec jekyll serve
```
- localhst:4000에 링크가 생겼다. 이 링크를 클릭해도 블로그에 들어갈 수 있다.
- 그 다음 다음 명령어로 remote에 올렸다.
```yml
git add *
git commit -m "first update"
git push origin main
```


## 2. 테마 변경 
- https://github.com/ejjoo/jekyll-theme-monos에서 monos테마를 zip다운로드 했다.
- 압축을 풀고 _post를 제외한 모든 파일을 복사했다.
- jylee529.github.io 디렉터리에 붙여넣고 같은 파일은 덮어쓰기를 했다.
- 그런데 bundle exec jekyll serve를 해도 링크가 뜨지 않아서 뭔가 잘못된 줄 알고 지우고 다른 방법으로 시도하기를 십수번 반복하다가 조교분께 여쭈었더니 푸시까지 하고 깃허브 링크에서 잘 뜨면 상관 없다고 하셨다.
- add commit push를 하고 깃허브 리퍼지터리 settings - pages 에서 링크로 들어가니까 제대로 테마가 적용되었다. 

## 3. _config 수정
- title과 description을 수정하였다.
```yml
title: blog of jy
description: >- 
  20223125 소프트웨어학부 이정윤
```

## 4. post추가 
- 테마를 잘못 고른 것 같다. post가 어떻게 해야 나오는지 모르겠다. 
- 테마를 바꾸기로 했다. 

## 5. 절망
- 망했다. 테마를 바꾸니까 화면이 완전히 깨져버렸다. 
- 지금까진 백업해놓은 기본 테마로 복구를 했는데 이젠 그것도 안되는것 같아 보인다.
- 결국 모두 삭제하고 리퍼지터리 만드는것 부터 다시 했다.
- 기본 테마로 복구하는데 성공했다. 
- 다른 테마를 아까 성공했던 방식대로 다운로드하고 붙여넣기 했다. 
- add commit push까지 했다. readme가 업데이트 된걸 보니 정상적으로 push된 것 같았다.
- 그러나 사이트는 기본테마에서 바뀌지 않았다. 
- 20시간 째 하나도 제대로 못하고 있는 꼴을 보니 아주 자살을 하고 싶다. 
- 다시 기본테마로 복구해보자.
- 기본테마로 복구하려고 했는데 수십개의 에러와 함께 push가 안 된다.
- 그냥 테마는 포기해야겠다. 벌써 5번째로 리퍼지터리를 삭제했다.
- 다시 처음부터 해서 기본테마로 복구했다. 그냥 여기다 하기로 했다.