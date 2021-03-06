# Linux

## 리눅스의 특징 및 기능

- 뛰어난 신뢰성, 동급 최고의 성능
- 다양한 업무 환경을 만족시키는 다양한 배포판의 존재
- 다중 사용자, 다중 처리 시스템
    - 각각의 응용 프로그램은 다른 응용 프로그램에 보호적으로 동작
    - 하나의 응용 프로그램 오작동이 전체 시스템을 다운시키는 것을 완벽하게 보호
- 풍부한 응용 프로그램의 제공
- 누구나 자유롭게 사용할 수 있는 운영체제
- 강력하면서 안정적인 네트워크 지원
- GUI 방식의 X 윈도우 지원
- 뛰어난 안정성과 보안성



## 디렉토리 
### 디렉토리 구조

```
/ - (root) - 최상위 디렉토리 , 모든 디렉토리의 출발점
|- bin      - 기본적인 명령어가 저장된 디렉토리. mv, cp, rm 같은 기초적인 명령어들 존재
|                 root 사용자와 일반 사용자가 함께 사용할 수 있음           
|
|- boot    - 리눅스 부트로더가 존재하는 디렉토리. GRUB와 같은 부트로더에 관한 파일들
|                 (grub.conf등)이 이 디렉토리에 존재
|
|- dev      -  시스템 디바이스 파일을 저장. 하드디스크 장치파일 /dev/sda, CD-ROM /dev/cdrom 
|                  등과 같은 장치파일들이 존재하는 디렉토리
|
|- etc       - 시스템의 거의 모든 설정 파일이 존재. ex) 시스템 제어판용, 사용자 관리 등
|
|- home  -  사용자 홈 디렉토리. useradd 명령어를 통해 새로운 사용자 생성 가능
|
|- lib        - 커널이 필요로하는 커널모듈 파일들과 프로그램에 필요한 각종 라이브러리 파일 존재
|
|- media  - DVD, CD-ROM, USB 등과 같은 탈부착이 가능한 장치들의 마운트 포인트로 사용됨
|
|- mnt     - media와 비슷한 용도로 탈부착 가능한 장치들에 대하여 **일시적**인 마운트 포인트로 사용
|
|- opt      - 크롬 브라우저, 안드로이드 스튜디오 등과 같은 써드파티 어플리케이션에 대한 설치 
|
|- proc    - `가상파일시스템`이라고 하는 곳으로 현재 메모리에 존재하는 모든 작업들이 파일형태로 
|                 존재하는 곳
|
|- root    -  시스템 최고 관리자인 root 사용자의 개인 홈 디렉토리. sudo -i 사용후 들어 갈 수 있음
|
|- run     -  계속 실행되고 있는 프로세스를 저장하고 있는 경로
| 
|- sbin    - 필수 시스템 바이너리 ex) init, ip, route. 주로 시스템 관리자들이 사용하는 시스템 
|                관리자용 명령어를 저장하고 있는 디렉토리
|
|- tmp    - 임시 파일. 시스템 사용하는 모든 사용자들이 공동으로 사용하는 디렉토리. mysql 에서 
|               사용하는 mysql.sock 등과 같은 소켓파일, 또는 아파치에서 사용하는 세션파일등이 
|               생성 되기도 함
|
|- usr     - 읽기 전용 사용자 데이터가 있는 보조 계층 구조. 주요(다중) 사용자의 유틸리티와 
|               어플리케이션 포함
|
|- var     - 시스템 운영중에 저장되는 자료가 저장되어 있는 경로
|
|- lost+found - 최상위 디렉토리인 `/` 디렉토리에만 존재하는 것이 아니라 파일 시스템마다 존재할 수 있는 디렉토리.
```

### [디렏토리 명령어](https://github.com/SYS-3th/Linux/blob/3f70a02a3cc4a73d92ce5b18f63ef49e8882f567/directory/directorylang.md)

## 상대경로와 절대 경로

### 절대경로
	기준 : 누구나 다 알고있는 동일한 위치를 기준으로 상대를 찾는 표현

	'/' 기준 -> '/' 는 웹사이트의 루트 폴더 > "http://localhost:8090" 

	'/WebClientTest' == 'WebContent'
### 상대경로

	기준 : 현재 웹페이지의 소속 폴더가 기준점

        . : 현재 웹페이지가 소속된 폴더

        .. : 현재 웹페이지의 부모 폴더

	자식폴더명 : 현재 소속된 폴더의 자식 폴더

	현재 위치를 '나'로 기준을 삼고 상대를 찾는 표현


## 파일

### [파일명령어](https://github.com/SYS-3th/Linux/blob/ecf2a0fc8ec26c8b4152081fde3c73e93d3c1676/file/filelang.md)

## 문서편집기 
### vi 편집기
- [vi명령어](https://github.com/SYS-3th/Linux/blob/da89c6ded7b4e913569c9eb40ef9e00273765b60/vilang.md)
### nano 편집기
- [nano 명령어](https://github.com/SYS-3th/Linux/blob/717121d6a4b2e022ddb019db0b7b12081142cef9/nanolang.md)
## 파일 및 디렉토리 검색 
## 파일내에서 검색

 ### [grep명령어](https://github.com/SYS-3th/Linux/blob/f90a429a6ac618922c23d9d737c40ef0d7926d9c/serch/grep.md)
 ### [fgrep명령어]()
## 디렉토리 내에서 감색

### [find](https://github.com/SYS-3th/Linux/blob/8915006a90a409e424904b96eaf650e82e050807/serch/findlang.md)
## 하드링크와 심볼릭 링크
윈도우로 치면 "바로가기" 같은 개념으로, 리눅스에도 링크 기능이 있다. 특정 파일이나 디렉터리를 링크 걸어 사용할 수 있는데, 링크에는 두 종료가 있다.
두 개 모두 처리하는 역할은 같지만 개념이 약간 다르다. 그 개념을 바로 잡고 적절하게 사용할 수 있어야겠다.

### harnlink
- 원본 파일과 동일한 inode 를 가지며 원본 파일이 삭제되더라도 링크 파일을 여전히 사용 가능하다
- ln [Source] [Target] 명령어로 생성 가능
- 위치 정보를 가지고 있는 이름을 여러 개 생성하는 개념이다. 그렇기 때문에 한 파일을 지워도 하드에서 해당 위치를 찾아갈 수 있다
### Symbolic Link
- 원본 파일의 이름을 가리키는 링크로 원본 파일이 삭제되면 사용 불가능하다
- 전혀 다른 파일이라도 가리키는 원본 파일 이름이 같으면 계속 사용 가능하다
- ln -s [Source] [Target] 명령어로 생성 가능. Source 를 가리키는 심볼릭 링크 Target 을 만든다
- Source 파일을 수정하면 심볼릭 링크인 Target 파일도 수정된다
- Target 파일을 수정해도 Source 파일이 같이 수정된다
- 위치 정보를 갖고 있는 파일명을 또 다른 이름으로 가리키는 포인터의 개념이다
- 하드링크는 한 위치 정보를 또 다른 이름으로 가리키는 개념
## 권한의 이해와 설정방법 

## 특수권한
[특수권한](https://github.com/SYS-3th/Linux/blob/3f5fe95e4665904c542de90fe59dde7a08a288b5/rights/special%20rights.md)

## 셀 명령어
### [쉘 명령어](https://github.com/SYS-3th/Linux/blob/3873c99b92ef2f311fab02b14ab2b9d46aa4f14d/shall/shall.md)
### [쉘 연산자](https://github.com/SYS-3th/Linux/blob/ba5604c6b9c89c2819f712adef8edb42e96cc05f/shellnu,/shellnum.md)
### [쉘_오늘날짜 저장하는 파일생성](https://github.com/SYS-3th/Linux/blob/5e6c316cd3a2848a9864c76b34b12044e9bbee6c/shall/shelltoday.md)

## 프로세스 제어

### [프로세스제어](https://github.com/SYS-3th/Linux/blob/16a6f06c6352fdab085a5bfacbe6fb01df56971a/process/process.md)

## 압축 및 아카이브
[아카이브 ](https://github.com/SYS-3th/Linux/blob/c22bebfd9bc30e4843f7e3762cbf66ceeeede4c8/archive/archive.md)

## 패키지 매니저 
 
[패캐지매니저](https://github.com/SYS-3th/Linux/blob/9c06e46754111423296fd704132f53dfe9ac8d43/pakage/package.md)

 
