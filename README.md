# homework
open source lecture homework repository


### Getopt 명령어
getopt 명령어 - 명령어 옵션을 분석할 수 있게 제공하는 시스템 호출이 getopt함수
                명령어 option 추출 함수
getopt는 첫 번째와 두 번째 인자는 main함수의 argc와 arg를 그대로 전달하고 세 번째 option에 제공하고자 하는 옵션을 전달한다. 
만약 'a' 'l'옵션을 전달하고자 한다면 'al'이라고 전달합니다.



### Getopts 명령어
쉘에서 명령을 실행할 때 옵션을 사용하는데 사용된 옵션은 다른 인수들과 마찬가지로 positional parameters 형태로 전달되므로 스크립트 내에서 직접 옵션을 해석해서 사용해야한다.
이때 옵션 해석 작업을 쉽게 도와주는 명령이 getopts이다.
옵션에는 short 옵션과 long 옵션이 있는데 getopts명령은 short 옵션을 처리합니다.
#### short 옵션의 특징
short 옵션은 다음과 같이 여러가지 방법으로 사용할 수 있다. 그러므로 getopts명령을 이용하지 않고 직접 옵션을 해석해 처리한다면 옵션 처리에만 스크립트가 복잡해질 수 있다.


```
$ command -a -b -c

#####옵션을 붙여서 사용할 수 있으며 순서가 바뀌어도 된다.
$ command -abc
$ command -b -ca

##### 옵션인수를 가질 수 있다.
$ command -a xxx -b -c yyy

##### 옵션인수를 옵션에 붙여 쓸 수가 있다.
##### 그러므로 다음은 위의 예와 동일하게 해석됩니다.
$ command -axxx -bcyyy

##### 옵션 구분자 '--' 가 올경우 우측에 있는 값은 옵션으로 해석하면 안된다.
$ command -a -b -- -c
```



