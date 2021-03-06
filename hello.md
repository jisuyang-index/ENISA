# hello git

## git 명령어 요약

- Commit
어떠한 주제의 변경사항들을 주석과 함께 로컬에 기록한다.

- Add 
저장하려는 파일들을 묶는다.

- Push
Local Repository(로컬 저장소)의 Stage(스테이지)에 있는 커밋들을 Remote Repository(원격 저장소)에 업로드한다.

- Clone
원격저장소를 로컬저장소에 복사한다.

## 파일의 내용 되돌리기

- 특정 파일의 내용을 마지막 커밋으로 돌리고 싶다면 해당 파일 선택 후 '코드 뭉치 버리기' 선택

## 브랜치 변경하기
- 브랜치란 : 기존 내용을 유지한 채 새로운 기능을 추가하고 싶을 때 사용한다.
- 체크아웃 : 특정 브랜치(혹은 커밋)으로 돌아가고 싶을 때 사용한다.
- 소스트리의 체크아웃 : 브랜치 이름을 더블 클릭하는 것 만으로도 체크아웃 가능하다.

## 병합하기 1
- 헤드 브랜치에 변경사항이 없고
- 병합 대상 브랜치가 헤드로부터 시작된 경우
- 아주 쉽게 병합 가능 = Fast-forward 

## 병합하기 2
- 헤드 브랜치에 추가적인 커밋이 생기는 경우
- 진짜 병합이 필요해 진다.
- 충돌이 안 나면 좋은데, 충돌이 나도 겁내지 말자.

## 오늘의 기분
- 내 기분과는 달리 하늘이 푸르다.

## 충돌 해결하기
- 제일 중요한 점 : 겁내지 말아요!
- 같은 파일을 병합 대상 두 커밋에서 동시 수정했을 경우 충돌이 날 확률이 높다!
- 에디터 사용, 혹은 SourceTree를 사용해서 충돌 해결 가능하다.

## 커밋 되돌리기

### reset
- 쉽지만 커밋이 날아간다.
- 강제 push가 필요하다.

### branch 만들어서 되돌리기
- reset과는 달리 내용이 사라지지 않는다.
- 장점 : 쉽다.
- 단점 : 트리가 지저분해진다.

### revert
- 역시 커밋은 없어지지 않는다. (히스토리를 남길 수 있다.)
- 장점 : 가장 기본적
- 단점 : 충돌이 날 수 있다.
- 해당커밋 지정

### revert2
- revert로 여러 커밋을 되돌리려면 최신부터 순서대로 revert 하자
- 그렇게 하면 충돌을 막을 수 있다.

## 커밋 덮어쓰기
- 필요하다면 이전 커밋 덮어쓰기도 가능
- 'commit --amend'
- 이미 push를 한 경우 'push-force'가 필요함

## stash
- 다른 브랜치로 체크아웃하기 전에 현재 작업내용을 저장하는 임시 저장소
- 유용하니 잘 사용하자.