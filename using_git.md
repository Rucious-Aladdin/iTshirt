## local 폴더 내에서 우클릭 -> git bash here

## git repository 초기화, .git 폴더 생성
```sh 
$ git init
```

## 사용자 정보 입력후 등록
```sh
$git config --global user.email "이메일주소"
$git config --global user.name "사용자이름"
```
## 사용자 정보 등록 확인
```sh
$git config --list
```

## 버전으로 만들 파일 선택
(1) 현재 경로내의 모든 변경사항 추가
```sh
$git add .
```

(2) 특정파일만 추가
```sh
$git add "파일이름"
```
(3) 현재 add 된 파일 확인
```sh
$git status
```
## commit -> 버전 업그레이드전 설명
(1) 기본 commit 명령어
```sh
$git commit -m "수정 내용 설명"
```
(2) commit 된 내역 확인
```sh
$git log
```

## 버전 되돌리기(commit 이전 버전으로 revision)
```sh
$git checkout "git log 입력시 등장하는 커밋 앞 식별자 7자리"
```
*바로 가장 최신 commit으로 되돌리기"
```sh
$git checkout -
```
**이명령어는 좀 위험하므로 웬만하면 쓰지 않도록 한다..

## 로컬 저장소 및 원격저장소 연결
```sh
$git remote add origin "연결할 저장소 레포지토리 주소"
```
## 커밋을 둘 장소 이름 짓기
```sh
$git branch -M main
```
## 원격저장소에 파일올리기
```sh
$git push origin main(브랜치 이름)
```
## 원격저장소의 커밋을 로컬 저장소에 내려받기
(1) 그자리에 바로 내려 받기(한칸 띄우고 마침표)
```sh
$git clone "저장소주소" .
```
(2) 폴더이름까지 통째로 내려받기
```sh
$git clone "저장소"
```

