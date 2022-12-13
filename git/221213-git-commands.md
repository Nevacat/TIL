# Git & Github

## Git 

### what is Git and Who maked Git?

 - `Git`은 'Linus Torvalds'가 만들었다.

 - `Git`은 '버전컨트롤시스템(VCM)'으로 사용자가 작성하고 수정한 것들의 버전을 관리한다.

### Git object

  `Blob` : 파일 하나의 내용에 대한 정보(사진으로 따지면 피사체)을 뜻한다.
 
  `Tree` : Blob이나 subtree의 메타데이터(디렉토리 위치, 속성, 이름 등 수정사항).
  
  `Commit` : 커밋 순간의 스냅샷

### Git Process Flow and Command

 **Local**

 working directory(내가 작업한 것들) -[git add]> staging area(커밋할파일의 정보들을 저장해두는 곳)

 staging area -[git commit]> localrepo(로컬 저장소)

 ```git
 git clone 주소 /* githun에서 만든 저장소의 주소를 가져온다. */
 touch .gitignore /* .gitignore라는 문서에 작성된 리스트는 git이 파일을 추적할 때 수정사항이 있어도 추척되지 않게 해준다.*/ 
 git status /* 현재  상태를 확인한다. */
 git add 파일명/* staging area에 코드의 변경사항들을 올려둔다.*/
 git commit /* localreop에 코드의 변경사항을 기록해둔다. */
 ```

 **Remote**
 
 localrepo -[git push]> remoterepo(원격 저장소)

 ```git
 git push origin main /* 커밋해둔 것들을 원격 저장소에 올려 저장한다.(팀원 또는 모든 사람들과  공유하게 된다.*/
 ```

### Conventional Commits

 1. commit의 제목은 commit을 설명하는 하나의 구나 절로 표현(문장X)
 2. Importance of Capitalize(* impotranceofcapitalize -> XXX *)
 3. prefix 꼭 달기
   - feat: 기능 개발 관련 (TIL에 기록하는 것들은 docs가 아닌 feat로 기록된다.)
   - fix: 오류 개선 혹은 버그 패치
   - docs: 문서화 작업 (README.md 등의 무언가를 설명할 때)
   - test: test 관련
   - conf: 환경설정 관련(.gitignore 등)
   - build: 빌드 관련
   - ci: Continuous Integration(지속적인 통합) 관련
 

## Github

 - Github는 Git을 이용하여 코드들을 저장하는 일종의 클라우드 저장소이다.
 - Git과 Github는 전혀 다른 것이다.

## LICENSE
 
 - 오픈소스 프로젝트에서 License는 내가 만들 때와 배포할 때 가장 신경써야되는 부분이다.

### Type of license

 - MIT License : MIT에서 만든 라이센스로 모든 행동에 제약이 없고 저작권자는 소프트웨어와 관련한 책임에서 자유롭다.

 - Apache license 2.0 : Apache 재단이 만든 라이센스로, 특허권 관련 내용이 포함되어 있습니다.

 - GNU General Public License V3.0 : 가장 많이 알려져있으며, 의무사항이 존재한다.(웬만하면 이 라이센스는  피해서 쓸 것)

