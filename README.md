# homework
open source lecture homework repository


Getopt 명령어
getopt 명령어 - 명령어 옵션을 분석할 수 있게 제공하는 시스템 호출이 getopt함수\명령어 option 추출 함수

getopt는 첫 번째와 두 번째 인자는 main함수의 argc와 arg를 그대로 전달하고 세 번째 option에 제공하고자 하는 옵션을 전달한다. 
만약 'a' 'l'옵션을 전달하고자 한다면 'al'이라고 전달합니다.



Getopts 명령어
쉘에서 명령을 실행할 때 옵션을 사용하는데 사용된 옵션은 다른 인수들과 마찬가지로 positional parameters 형태로 전달되므로 스크립트 내에서 직접 옵션을 해석해서 사용해야한다.
이때 옵션 해석 작업을 쉽게 도와주는 명령이 getopts이다.
옵션에는 short 옵션과 long 옵션이 있는데 getopts명령은 short 옵션을 처리합니다.
short 옵션의 특징
short 옵션은 다음과 같이 여러가지 방법으로 사용할 수 있다. 그러므로 getopts명령을 이용하지 않고 직접 옵션을 해석해 처리한다면 옵션 처리에만 스크립트가 복잡해질 수 있다.
