---
title: venv를 사용하여 Python 가상환경 작업
date: 2024-01-17 14:11:55 +09:00
categories: [dev_note]
tags: [python]
---

# venv
venv는 격리된 파이썬 환경을 만드는 도구이다.<br/>
로컬에서 작업시 전역 파이썬 환경과 종속항목(패키지들)이 꼬일 수 있으므로, 각 작업영역의 env 폴더에 패키지들을 격리시켜 준다.<br/>
근데 이러면 용량이 늘어날 수 있으니 틈틈히 신경 써야 할듯..?

## 가상환경 만들기
```shell
cd your-project
python -m venv env
```
위 코드는 venv 명령어를 사용하여 전체 Python 설치의 가상 복사본을 만든다. ```env```라는 폴더에 가상 복사본을 만들지만, 폴더 이름을 다르게 지정할 수도 있다.

## 가상환경 활성화
```shell
source env/bin/activate
```
터미널에서 앞에 (env)문구가 들어가서 가상환경이라는 것을 명시해준다.<br/>
```
(env) superkind@superk-MacBookPro:app-engine-python-test $ 
```

## 작업 시작!
이제 pip install와 같이 종속성을 설치하게 되면 가상환경(env 폴더)에서만 설치가 된다.

## 작업 중단
```
deactivate
```
가사환경을 중단하고 싶으면 이걸 쓰면 된다. 간단해..