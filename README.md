# Lab 11: Make a package called "geo"

`11_python2.pdf` 14쪽의 Python 패키지 과제입니다.

## 파일 구성

```text
geo/
    __init__.py
    utils.py
tester.py
```

- `geo/utils.py`: 직각삼각형의 빗변 길이를 반환하는 `pythagoras(a, b)`와 원의 넓이를 반환하는 `circle(r)`를 정의합니다.
- `geo/__init__.py`: 패키지를 초기화하고 `__all__`에 두 함수를 지정합니다.
- `tester.py`: `import geo.utils as utils`로 모듈을 불러와 수업 예제의 두 계산을 실행합니다.

## 실행

Python 3에서 저장소 폴더를 열고 실행합니다. 표준 라이브러리 `math`만 사용하므로 별도 패키지 설치는 필요하지 않습니다.

```sh
python tester.py
```

출력:

```text
c = 5.0
area = 314.1592653589793
```

`pythagoras(3, 4)`는 피타고라스 정리를 이용해 빗변 길이 5.0을 반환하고, `circle(10)`은 반지름이 10인 원의 넓이인 100π를 반환합니다.
