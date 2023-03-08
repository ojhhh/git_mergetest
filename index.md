# git 다시 해보기

## 새 저장소 만들기

- git init

## 파일 전부 스테이징

- git add .

## 커밋 메시지 작성

- git commit -m "작업 내용"

## github 원격저장소 연결

- git remote add origin "저장소 주소"

## 파일 업로드

- git push origin main

## 브런치 영역 나누기

## 브런치 : 저장소의 작업 공간

- master는 최종 작업물. 다른 브런치를 만들어 여렀이서 작업을 하거나 혼자 작업할 때 작업의 내용을 나눠서 작업 하고 최종 작업물로 병합
- dev 브런치를 만들어 작업하다 최종적으로 master에 병합.
- 순서 : master(v0.1) -> dev -> master(v0.2) 병합
- master -> dev1, dev2 -> dev1 + dev2 -> dev1 + master

## 브런치 목록 확인

- git branch : 로컬 저장소의 브런치 목록 확인
- git branch -a : 원격 저장소와 로컬 저장소 브런치 목록 확인
- 선택되어 있는 브런치는 \*(이름) 으로 표시

## 브런치 생성

- git brach (생성할 브런치의 이름)
- ex) git branch branchtest

## 브런치 이동

- git checkout (이동 브런치 이름)
- ex) git checkout branchtest
- git switch (이동할 브런치 이름)
- ex) git switch branchtest

## 저장소 병합

- git merge (병합할 브런치 이름)

## merge 병합 중 충돌

## 브런치 제거

- git branch -d (제거할 브런치 이름)
- ex) git branch -d branchtest

## 브런치 생성 후 push를 해서 원격 저장조에 브런치 생성

- git branch dev
- git pull origin dev -> Fatal: couldn't find remote ref dev
- git branch -a
- \* dev
- main
- remotes/origin/main
- git push origin dev
- git pull origin dev -> 성공
- git branch -a
- \* dev
- main
- remotes/origin/dev
- remotes/origin/main
