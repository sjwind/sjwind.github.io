# Online Jupyter Notebook for Python





## Google Colab vs. MS Azure Notebook vs. Binder



Online 환경에서 데이터 분석을 진행할 수 있는 대표적인 플랫폼을 비교/평가 해 보았다. 



1) Google Colab

2) MS Azure Notebook

3) Binder



다양한 측면에서 비교를 할 수 있지만, 진정으로 크리티컬한 부분에서 놓칠 수 없는 비교점이 있다. 







## Google Colab



제공되는 리소스는 ```2 CPU, 12G Mem 할당``` 으로 상당히 준수하다. 게다가 GPU를 제공해 주고 있어서, GPU 모드로 ML 연산을 계산할 수 있다. 



Google Colab에서 제공하는 리소스 스펙

CPU 스펙

```python
!cat /proc/cpuinfo
```

```python
processor	: 0
vendor_id	: GenuineIntel
cpu family	: 6
model		: 79
model name	: Intel(R) Xeon(R) CPU @ 2.20GHz
stepping	: 0
microcode	: 0x1
cpu MHz		: 2200.000
cache size	: 56320 KB
```

Memory 스펙

```python
!free -h
```

```python
              total        used        free      shared  buff/cache   available
Mem:            12G        3.0G        7.4G        908K        2.3G         11G
Swap:            0B          0B          0B
```







### 장점

웹환경에서 실행하여줌에도 불구하고, GPU를 지원해줌

ML을 구동시키기에 적당함



### 단점

UI가 몹시 레거시함





![image-20200515152247703](/Users/audit01/Library/Application Support/typora-user-images/image-20200515152247703.png)

개인차이가 있을 수 있겠으나, UI 좀 덜 아름답다. 뭔가 과거의 파워빌더(PowerBuilder)를 보는 느낌이랄까?



![img](https://k.kakaocdn.net/dn/ca9bkW/btqEcnRjWTI/KRiP5gdMZI9ILBK8KEBDF0/img.png)

실행할 때 마다 차이가 존재한다. 2~3번째 실행 할 때는 1.83초





## Microsoft Azure Notebook



MS Azure Notebook의 제공되는 리소스의 스펙

```python
!cat /proc/cpuinfo
```

```python
processor	: 0
vendor_id	: GenuineIntel
cpu family	: 6
model		: 79
model name	: Intel(R) Xeon(R) CPU E5-2673 v4 @ 2.30GHz
stepping	: 1
microcode	: 0xffffffff
cpu MHz		: 2294.689
cache size	: 51200 KB
```



```python
!free -h
```

```python
              total        used        free      shared  buff/cache   available
Mem:           3.8G        568M        3.1G         17M        198M        3.0G
Swap:            0B          0B          0B
```







### 장점

UI 측면에서 Jupiter Notebook 그대로를 사용하고 익숙할 뿐만아니라, UI의 편의성과 활용성이 더욱 사용하기 좋음

Python 버전별로 커널을 생성하기에 편리하며, Python 외 R 등 환경도 잘 디플로이 되어 있음

다양한 강좌들을 포함하고 있어서, 공부하는데 많은 도움이 됨



### 단점

파일 접근 할 때 속도가 많이 느림.









![img](https://k.kakaocdn.net/dn/eqquwR/btqEdw7BsC4/0FUvpp7iezQhnC2p6ejoRK/img.png)

두번째 및 3번째 실행 시 15.37초







## Binder





자체적으로 notebook을 작성하여 사용하는 방식이 아닌, GitHub에 있는 Repository를 가져와 서 실행 시켜주는 방식이다. 





![img](https://mybinder.org/static/logo.svg?v=f9f0d927b67cc9dc99d788c822ca21c0)



![image-20200515153550284](/Users/audit01/Library/Application Support/typora-user-images/image-20200515153550284.png)









```python
!cat /proc/cpuinfo
```

```python
processor	: 71
vendor_id	: GenuineIntel
cpu family	: 6
model		: 85
model name	: Intel(R) Xeon(R) Gold 6140 CPU @ 2.30GHz
stepping	: 4
microcode	: 0x2000064
cpu MHz		: 1000.027
cache size	: 25344 KB
```







Memory 스펙

```python
!free -h
```

```python
              total        used        free      shared  buff/cache   available
Mem:           754G         52G        101G         15M        600G        705G
Swap:            0B          0B          0B
```







## GitPod













CPU 스펙

```python
!cat /proc/cpuinfo
```

```python
processor       : 15
vendor_id       : GenuineIntel
cpu family      : 6
model           : 79
model name      : Intel(R) Xeon(R) CPU @ 2.20GHz
stepping        : 0
microcode       : 0x1
cpu MHz         : 2200.000
cache size      : 56320 KB
```

M



Memory 스펙

```python
!free -h
```

```python
              total        used        free      shared  buff/cache   available
Mem:           58Gi       8.3Gi        23Gi       4.0Mi        27Gi        51Gi
Swap:            0B          0B          0B
```













































