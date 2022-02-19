KoPy (Korean Python)
========

파이썬 한국어 형태소 분석기입니다.
- 블로그 : https://biggydog.github.io/python/

#### 설치방법
- pip install kopy

#### 사용방법
##### python 3
```python
from kopy import KoPy
kp = KoPy()
kp.pos('안녕하세요!')
  [('안녕', 'NNG'), ('하', 'XSA'), ('세요', 'EF'), ('!', 'SF')]
kp.sentence('안녕하세요! 반갑습니다.')
  ['안녕하세요!', '반갑습니다.']
```
##### python 2
```python
from kopy import KoPy
kp = KoPy()
kp.pos('안녕하세요!')
  [(u'\uc548\ub155', u'NNG'), (u'\ud558', u'XSA'), (u'\uc138\uc694', u'EF'), (u'!', u'SF')]
kp.pos('안녕하세요!',1)
  ('안녕', 'NNG'), ('하', 'XSA'), ('세요', 'EF'), ('!', 'SF')
kp.sentence('안녕하세요! 반갑습니다.')
  [u'\uc548\ub155\ud558\uc138\uc694!', u'\ubc18\uac11\uc2b5\ub2c8\ub2e4.']
kp.sentence('안녕하세요! 반갑습니다.',1)
  ('안녕하세요!'),('반갑습니다.')
```
