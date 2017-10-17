KoPy (Korean Python)
========

파이썬 한국어 형태소 분석기입니다.
- 블로그 : https://biggydog.github.io/python/

###설치방법
- pip install kopy

사용방법
```{.python}
from kopy import KoPy
kp = KoPy
kp.pos('안녕하세요!')
  [('안녕', 'NNG'), ('하', 'XSA'), ('세요', 'EF'), ('!', 'SF')]
kp.sentence('안녕하세요! 반갑습니다.')
  ['안녕하세요!', '반갑습니다.']
'''
