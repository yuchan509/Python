# Python
Python

### 파이썬 개요

#### 파이썬 구성

#### 개발 환경 구축
- 기본 IDE(Integrated Development Environment) 
  - python.org 접속후 특정 버전 다운로드.
    - 3.6.xx 이상.
    - 윈도우에서 사용.
    - 설치(로컬PC).
  - 리눅스상에서 설치.( 도커(가상환경 : 로컬) or AWS(아마존) ) => 패키지 관리자를 통해 설치.
    - Linux(우분투 18.x) 에서는 기본적으로 2.7.xx 버전과 3.6 or 3.7 버전이 기본적으로 설치됨.


- 풀패키지 설치
  - Anaconda or Miniconda
    - 필요한 모든환경, 패키지를 다 설치. 
    - 다운로드 후 설치.(로컬PC)
    - 윈도우 설치시 path 체크 수행할 것.
    - Anaconda 네비게이터에서 개발 환경에 진입.(직접 접근도 가능함)
    - 프로젝트에 맞춰서 환경 탭에서 가상 환경을 하나씩 구성. : 샌드박스 모델
      - 각각의 가상환경은 서로 영향을 미치지 않음. : 프로젝트로 한개의 PC에서 수행하다 보면 패키지의 버전들이 충돌날 수도 있음 
      - 따라서 가상환경은 독립된 개발 환경을 제공한다는 장점을 가짐.
      - virtualenv라는 패키지가 제공.
      - Linux 상에서는 직접 구축.
      - Anaconda는 메뉴로 제공(빌트인)

- 클라우드 기반   
  - 구글의 Colab 등(브라우저에 접속하여 개발.)
      - 제공받은 환경에서 개발.
      - GPU, TPU등 지원.(12시간 사용 가능.)
      - 개발 IDE는 Jupyter Notebook을 이용.
      - 원래 데이터 분석용 패키지: iPython
      - Jupyter Notebook이라는 웹 기반 분석용 모듈을 지원.
      - 대화형으로 개발, 1줄 1줄에 집중하는 방식.
      - 작업 파일. => ipynb
      - 기반 OS : Linux 우분투 18.04v

#### Editor 혹은 IDE
- 전용 IDE
  - PyCharm, PyDev,.....Pyxx
- 범용 IDE
  - **Vs code**, visual studio, eplise,...




### 파이썬 목차
#### 단일 타입 자료형 : 데이터 본질
- 수치형
  - 정수형.
    - ..., -1, 1, 0, ...
    - 이진수, 8진수, 10진수, 16진수,...
  - 부동소수형
    - 3.14
    - 소수부가 존재하는 타입.
    
- 블린형.
  - True, False
  
- 문자열, 수정불가.
  - '가나다', "가나다"
  - '''가나다''', """가나다"""


#### 연속 타입 자료형
- 특징 : 단일 데이터를 n개를 모아서 일괄적으로 다양하게 관리하는 자료형, 연속형, 시퀀스타입.
- Pyhton
  - 문자열
  - 리스트   : [], **list**, 순서 O, 중복값 허용.
  - 딕셔너리 : {}, **dict**, 순서 X, 키, 값의 세트로 존재, 키는 중복 불가, 값은 중복허용
  - 튜플     : (), **tuple**,순서 O, 중복O, 단순하게 데이터를 묶는다, 수정불가.
  - 집합     : {}, **set**, 순서X, 중복제거. 

- 넘파이(numpy) : 수학/과학용 라이브러리.
  - 배열 => 행렬 : **ndarray**, 동일 타입으로 데이터가 존재, 스칼라, 백터 용어 등장, n차배열.

- 판다스(pandas) : 데이터 사이언스: 분석,통계 용 라이브러리 <->  R과 대응.
  - 시리즈 : **Series**, 동일타입, 1차배열 + 인덱스
  - 데이터 프레임 : **DataFrame**, 컬럼별 타입은 동일, 2차배열 + 인덱스 + 컬럼

- 딥러닝 : 엔진 or 프레임웍(Tensorflow, PyTorch, keras)
  - Tensor => 행렬 연산 : **Tensor**, 데이터는 모두 수치(정수, 부동소수만 존재), 1차, 2차, 3차,..n차 텐서


#### 조건문, 반복문, 제어문  :  흐름제어
- 제어문 : if, elif, else
- 반복문 : for, while
- 조건문 : 조건 연산자
 - 조건문의 결론은 True/False
 - False 상황을 기억.


#### 절차적 프로그래밍
- 타입, 조건문, 반복문, 제어문 등을 이용하여 특정 주제의 SW 개발.
- 타입, 조건문, 반복문, 제어문 숙련.
- SW 개발 방식 숙련.
- IDE : Vs code 사용.


#### 함수
- 역활과 의미
- 사용자 정의 함수
- 내장 함수
- 외장 함수
- 람다 함수 : 가장 빠름.
- 클로저
- 기타 고급표현


#### 함수 지향적 프로그래밍
- 함수 지향적으로 프로그램을 작성함으로써 얻는 이득과 장점을 이해.
- 절차적 => 함수 지향적으로 전환하면서 기술에 대한 이해.


#### 클래스
- 클레스 정의와 의미.
- 상속과 맴버구성.
- GUI, 딥러닝 Keras에서 많이 이용.
  - 만들기 나름.

#### 객체 지향적 프로그래밍
- Game 개발 part 참고.

#### 모듈 및 패키지
- 모듈(파이썬 파일:*.py) 
- 패키지(디렉토리, 같은 계열의 모듈을 계층적으로 관리.)
- 내가 만든 모듈 혹은 패키지를 다른 사람이 사용한다면 어덯게 구성 하고, 가져다 사용할 수 있는가
- Game 개발 part 참고.

#### 예외처리
- s/w 죽으면 안됨.
- 오류가 발생할 만한 곳에 예외처리를 수행.
- 발생할 만한 대부분은 위치는 I/O 처리시 발생.
- try ~ : 5가지 처리 형태가 존재.
- 위의 기능을 조합해서 흐름제어를 완성.
- 
#### 기타 고급 표현
- 정규식
