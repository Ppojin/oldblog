---
title: python virtualenv
tags: python
---

## 개요
virtualenv 는 파이썬 라이브러리를 독립적으로 만들어 줄 수 있는 라이브러리이다.

## 설치
```
$ pip install virtualenv
Collecting virtualenv
  Using cached https://files.pythonhosted.org/packages/8b/12/8d4f45b8962b03ac9efefe5ed5053f6b29334d83e438b4fe379d21c0cb8e/virtualenv-16.7.5-py2.py3-none-any.whl
Installing collected packages: virtualenv
Successfully installed virtualenv-16.7.5
```

## virtualenv 환경 설치
터미널에 `virtualenv env` 를 입력하면 현재 폴더에 env폴더가 생성된다.
```
$ virtualenv env
Using base prefix '/Library/Frameworks/Python.framework/Versions/3.7'
New python executable in /Users/hwanghyojin/Documents/flask/makeservay/env/bin/python3
Also creating executable in /Users/hwanghyojin/Documents/flask/makeservay/env/bin/python
Installing setuptools, pip, wheel...
done.
```

## virtualenv 환경 실행
`source env/bin/activate` 명령어를 실행하면 virtualenv 가상 환경에서 작업을 진행할 수 있다.
bash 뒤에 (env)가 붙으면 가상 환경이 동작중이라는 표시이다.
```
$ source env/bin/activate
(env) $
```

## virtualenv 환경 종료
virtualenv 가상 환경이 실행 중일 때 `deactivate` 명령어를 입력하면 가상 환경에서 나와 local 환경에서 작업할 수 있다.
```
(env) $ deactivate
$
```