# ADC 레지스터를 이용한 단순 센서데이터 수집

### STM32F429ZI사용, NTSF-4 써미스터(온도센서) 이용

![Image](https://github.com/user-attachments/assets/3e6ddac2-df71-4f5e-b22f-171de6bc212c)

1. 폴링 방식 접근

2. 전압값으로 변경 후 온도값 출력을 위한 수식 성립
식을 증명 한다면, NTC써미스터로서, 온도가 증가하면 저항이 감소하는 특성을 가지기에, 식을 세우면 이렇게 지수 함수로 표현 된다..

<img width="2385" height="984" alt="beta_equation_ln" src="https://github.com/user-attachments/assets/6c341432-f4d0-4aeb-b061-0fa8de256008" />

우리가 원하는 것은 현재 온도 T이기에, 이 T를 구하기 위해서는 지수함수를 선형 함수로 바꿔야 하기에, 곱셈 로그 공식을 사용한 후 양변에 대해 정리하면 온도 T를 구할 수 있다.
고로 나온 식은.

<img width="597" height="129" alt="image" src="https://github.com/user-attachments/assets/b542a573-8bda-4419-b88c-c255d33f5d0c" />



하지만, 이 온도는 화씨이므로, 섭씨로 변경하기 위해선, 도출된 온도에서 -273.15를 뺀다.

<img width="525" height="488" alt="image" src="https://github.com/user-attachments/assets/1dc82a9d-174e-4396-9cb0-ffec47e561e5" />
