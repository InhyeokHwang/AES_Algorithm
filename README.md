# AES_Algorithm
This is modified version of kokke's AES algorithm to make it easier for me to use.
https://github.com/kokke/tiny-AES-c

사용하고자 하는 key 사이즈 선택 (aes.h 헤더파일의 27~29번째 줄) 

![image](https://user-images.githubusercontent.com/91961916/211988610-249e3d14-e221-4538-8c14-1dd27d536fbd.png)

1.	ECB mode 에서 Encrypt 하고자 할 경우

![image](https://user-images.githubusercontent.com/91961916/211988785-1940db81-4f0a-44c9-b284-eb47fc1904ed.png)

Key 배열에 키 값을 입력

In 배열에 평문을 입력 (한 줄이 16바이트가 되도록 개행 되어있으며, 평문이 16바이트의 배수가 아니라면 상황에 맞는 패딩을 직접 추가하여 16바이트의 배수로 만들 것)

2.	ECB mode 에서 Decrypt 하고자 할 경우 

![image](https://user-images.githubusercontent.com/91961916/211988839-fe21bc21-830e-4d7d-bb2e-a8328a45d73a.png)

Key 배열에 key 값을 입력

In 배열에 복호화할 암호문을 입력(한 줄이 16바이트가 되도록 개행 되어있으며, 암호문이 16바이트의 배수가 아니라면 상황에 맞는 패딩을 직접 추가하여 16바이트의 배수로 만들 것)

3.	CBC mode 에서 Encrypt 하고자 할 경우 

![image](https://user-images.githubusercontent.com/91961916/211988888-30e14307-a642-4aac-b853-431b87f39c3c.png)

Key 배열에 키 값을 입력

Iv 배열에 initialize vector 값을 입력
In 배열에 평문을 입력 (한 줄이 16바이트가 되도록 개행 되어있으며, 평문이 16바이트의 배수가 아니라면 상황에 맞는 패딩을 직접 추가하여 16바이트의 배수로 만들 것)

4.	CBC mode 에서 Decrypt 하고자 할 경우 

![image](https://user-images.githubusercontent.com/91961916/211988966-b67c0f30-c237-478b-be7e-bc4fe446074f.png)

![image](https://user-images.githubusercontent.com/91961916/211988982-5160a898-d0bd-4692-9f82-9fbdf1b3570a.png)

Key 배열에 key 값을 입력

Iv 배열에 initialize vector 값을 입력
In 배열에 복호화할 암호문을 입력(한 줄이 16바이트가 되도록 개행 되어있으며, 암호문이 16바이트의 배수가 아니라면 상황에 맞는 패딩을 직접 추가하여 16바이트의 배수로 만들 것)

AES128테스트 출력 결과:

![image](https://user-images.githubusercontent.com/91961916/211989044-5df29cd9-ce65-4687-ac6b-0b6399fc6d24.png)
