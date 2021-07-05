# Git

> git에 대해 학습한다.

---

[TOC]

---



## 사용이유

- **변경 내용을 추적**하기 위해 사용한다.



## git bash

- linux 언어 사용 가능



## 사용자 등록

> git bash 최초로 설치하면, **처음에 딱 한 번만** 사용자 정보를 등록해준다.

1. username

```bash
$ git config --global user.name "ijua9774"
```

2. user email

```bash
$ git config --global user.email ijua9774@naver.com
```

**확인하기**

```bash
$ git config --global user.name
$ git config --global user.eamil
```

- 혹은 아래의 명령어로 설정 정보를 모두 확인할 수 있다.

```bash
$ git config --list
```



## git 기본 명령어

> 시작하기 전 해당 폴더가 git으로 관리되고 있지 않다면, git 폴더로 만들어준다.
>
> ```bash
> $ git init
> ```

1. add

```bash
$ git add <파일명>
```

- 보통은 다음과 같이 사용한다.

  ```bash
  $ git add .
  ```

  - 현재 폴더 아래의 모든 파일 및 폴더를 add한다.

2. commit

> stage에 변경사항을 올린다.

```bash
$ git commit -m "<메시지 내용>"
```

- 메시지는 임의로 입력할 수 있다.
- :ballot_box_with_check: 내가 변경사항을 알아볼 수 있도록 commit message를 입력해주면 좋다!

3. push

> 원격저장소(네트워크에 있는 git repository)에 변경내용을 올린다.

```bash
$ git push origin master
```

- origin - 내가 설정한 원격저장소 이름 (임의)
- master - 내가 설정한 브랜치 이름 (임의, **default**)



## git 추가 명령어

**원격저장소 연결하기**

- git repository의 원격저장소와 연결한다.
- git repository의 `Code > HTTPS주소`를 복사한다.

```bash
$ git remote add <원격저장소 별칭> <주소>
```

- 보통 다음과 같이 사용한다.

```bash
$ git remote add origin <주소>
```

**다른 사람 git 가져오기 (git clone)**

- 원하는 repository의 주소(https 주소)를 복사한다.
- 원하는 폴더에서 bash를 실행해준다.

```bash
$ git clone <주소>
```

