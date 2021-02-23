## 시작합니다


# 이건 뭐다?


### 이건?


```python
#split
a='hello world nice weather'
b=a.split()
print(b)
```

    ['hello', 'world', 'nice', 'weather']
    


```python
#replace
b[1]
d=b[1].replace('w','W')
print(d)
```

    World
    


## extend란 무엇인가


```python
#extend 리스트 연장
a=[1,2,3,4,5]
b=[5,4,3,2,1]

a.extend(b)
print(a)
```

    [1, 2, 3, 4, 5, 5, 4, 3, 2, 1]
    


```python
#pop 지우고 반환
a=[1,2,3,4,5]
d=a.pop(2)

print(a)
print(d)
```

    [1, 2, 4, 5]
    3
    


```python
#list 정렬
a=[9,19,7,24]
b=sorted(a)
a.sort(reverse=True)

print(a)
print(b)
```

    [24, 19, 9, 7]
    [7, 9, 19, 24]
    


```python
#딕셔너리 업데이트
a={'a':1,'b':2,'c':3}
b={'a':100,'d':200,'e':300}

a.update(b)
print(a)
```

    {'a': 100, 'b': 2, 'c': 3, 'd': 200, 'e': 300}
    


```python
#딕셔너리 키,값 반환
print(a)
print(list(a.keys()))
print(list(a.values()))
list(a.items())
```

    {'a': 100, 'b': 2, 'c': 3, 'd': 200, 'e': 300}
    ['a', 'b', 'c', 'd', 'e']
    [100, 2, 3, 200, 300]
    




    [('a', 100), ('b', 2), ('c', 3), ('d', 200), ('e', 300)]




```python
#집합
a={1,1,2,3,3,4}
print(a)
```

    {1, 2, 3, 4}
    


```python
#집합 연산
a={1,2,3}
b={2,3,4}

print(a.union(b))#합집합
print(a.intersection(b))#교집합
print(a.difference(b))#차집합
print(a.issubset(b))#부분집합
```

    {1, 2, 3, 4}
    {2, 3}
    {1}
    False
    


```python
#while문 if문

a=[1,10,9,24,25,26]
i=0

while i<len(a):
    if a[i]%2:
        print(a[i])
    else:
        print(a[i]/2)
    i+=1
```

    1
    5.0
    9
    12.0
    25
    13.0
    


```python
#딕셔너리 출력
a={'korea':'seoul','japan':'tokyo','canada':'ottawa'}
for key in a:
    print(key,a[key])
for i in a.values():
    print(i)
```

    korea seoul
    japan tokyo
    canada ottawa
    seoul
    tokyo
    ottawa
    


```python
#for문 출력 인덱스 값 모두 사용
a=[1,2,3,4,5]
for i,val in enumerate(a):
    print(i,val)
```

    0 1
    1 2
    2 3
    3 4
    4 5
    


```python
#range(쉽게 리스트 만들기)
range(2,10)
```




    range(2, 10)




```python
#lambda함수(구현체만 존재하는 일회성 함수)
square=lambda x:x**3
square(2)
```




    8




```python
#class
#속성(attribute)와 동작(method)를 갖는 데이터 타입
#데이터(변수)와 다루는 연산(함수)를 하나로 다루는걸 클래스

```


```python
#object
#클래스로 생성되어 구체화된 객체(인스턴스)
#실제로 class가 인스턴스화 되어 메모리에 상주하는 상태
#class가 빵틀이라면, object는 실제로 빵틀로 찍어낸 빵이다

```


```python
class person:
    pass
bob=person()
cathy=person()

a=list()
b=list()

print(type(bob),type(cathy))
print(type(a),type(b))
```

    <class '__main__.person'> <class '__main__.person'>
    <class 'list'> <class 'list'>
    


```python
#__init__(self)

class Person:
    def __init__(self):
        print(self, 'is generated')
        self.name='kate'
        self.age=10
        
p1=Person()
p2=Person()

p1.name='Aragon'
p1.age=3552

print(p1.name,p1.age)
print(p2.name,p2.age)
```

    <__main__.Person object at 0x0000020BBE2FA978> is generated
    <__main__.Person object at 0x0000020BBE2E0D68> is generated
    Aragon 3552
    kate 10
    


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```
