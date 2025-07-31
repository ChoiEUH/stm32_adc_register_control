# ADC 레지스터를 이용한 단순 센서데이터 수집

### STM32F429ZI사용, NTSF-4 써미스터(온도센서) 이용

![Image](https://github.com/user-attachments/assets/3e6ddac2-df71-4f5e-b22f-171de6bc212c)

1. 폴링 방식 접근

2. 전압값으로 변경 후 온도값 출력을 위한 수식 성립
식을 증명 한다면, NTC써미스터로서, 온도가 증가하면 저항이 감소하는 특성을 가지기에, 식을 세우면

<img width="142" height="32" alt="image" src="https://github.com/user-attachments/assets/0e3c3600-6a67-4463-9808-f1211513bef7" />
이렇게 성립 된다.

<img width="525" height="488" alt="image" src="https://github.com/user-attachments/assets/1dc82a9d-174e-4396-9cb0-ffec47e561e5" />
