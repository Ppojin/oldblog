---
layout: post
title: 경험해본 python 개발환경 중 최고, jupyter notebook. 소개, 설치, 실행
description: jupyter notebook은 python이 인터프리터 언어인 점을 이용해서 실시간으로 코딩할 수 있는 개발환경입니다.
---

[Jupyter Notebook github 링크](https://github.com/jupyter/notebook)

# 소개
파이썬은 **인터프리터 언어**로써, ios의 **터미널**이나 윈도우의 **CMD**와 같은 커맨드 라인 창에서, 명령어를 이용해 실시간으로 작동하는 프로그래밍 언어입니다.

하지만 이런 특성을 이용하지 않는다면 **파이썬** 은 **C** 와 같은 컴파일 언어처럼 **IDE** 또는 **텍스트 편집기**를 이용해서 `<파일명>.py` 파일을 만들어서 저장하고, 일일히 **커멘드 라인**에서 `python <파일명>.py` 와 같은 명령어를 이용해 테스트하며 개발합니다.

하지만 파이썬 은 인터프리터 언어이기 때문에, 이런 특성을 이용한 **jupyter notebook** 을 이용해서 코딩을 한다면 에러가 없는지 테스트를 하기 위해 `python <파일명>.py` 과 같은 명령어를 입력하기 위해 일일히 커맨드창을 켤 일이 없습니다.

> ![img/cmd.PNG](https://raw.githubusercontent.com/Ppojin/Ppojin.github.io/master/blog/_posts/img/cmd.PNG)
파이썬 은 인터프리터 언어이다.
{:.figure}

# 설치
**pip** 명령어를 이용해서 **파이썬** 에 **notebook** 라이브러리를 설치합니다.
```
$ pip install notebook
```

jupyter 명령어를 이용해서 notebook을 실행합니다.
```
$ jupyter notebook
```

cd 명령어 등을 이용해서 원하는 폴더에서 notebook을 실행할 수도 있습니다.
```
~$ cd <폴더경로>
<폴더경로>$ jupyter notebook
```


> **NOTE**: 요세미티 이상의 맥os 유저의 경우 설치 후 `$ jupyter notebook` 명령어를 통해 실행할 때 `ImportError: cannot import name _thread` 와 같은 오류가 발생할 수 있습니다. 그럴 경우 *dateutil* 라이브러리를 2.2 버전으로 **재설치**하는 것 으로 이 문제를 해결할 수 있습니다.
>{:.message}
>
```
sudo pip uninstall python-dateutil
sudo pip install python-dateutil==2.2
```