# 3.1 산업용 통신 펌웨어 설정.

사용하기 위한 산업용 통신 펌웨어를 설정하는 방법은 다음과 같습니다. 설정이 완료 후 펌웨어를 적용하기 위해서는 제어기 전원을 차단한 후 다시 공급해주시기 바랍니다.

<br>

##### 1. 메뉴를 터치하여 펌웨어 설정 화면으로 진입 합니다.
**\[시스템 > 2: 제어 파라미터 > 11: 산업용 통신 > 1: 펌웨어 설정 > 1 채널]** 


<br>

##### 2. 아래 화면을 참고하여 슬롯과 통신 방식(Master/Slave), 프로토콜을 선택 합니다.
   * 슬롯 번호는 PCI 통신 카드의 Rotary Swtich 번호 입니다.
   * 통신 펌웨어 설정을 원하지 않을 경우 **\[OK]** 버튼을 터치하여 종료합니다.

{% hint style="warning" %}
**\[주의]**: **\[초기화]** 또는 **\[적용]** 버튼을 터치하면 현재 보고있는 탭의 펌웨어 정보가 초기화 됩니다. Config 파일도 같이 초기화 되니 유의하시기 바랍니다.
{% endhint %}

![[그림 3.1-1 산업용 통신 설정 화면]](<../_assets/3-Settings-Industrial-Communication/3.1-Setting-Firmware/image_1.png>)

![[그림 3.1-2 산업용 통신 설정 화면(master)]](<../_assets/3-Settings-Industrial-Communication/3.1-Setting-Firmware/image_2.png>) ![[그림 3.1-3 산업용 통신 설정 화면(Slave)]](<../_assets/3-Settings-Industrial-Communication/3.1-Setting-Firmware/image_3.png>)

<br>

##### 3. 펌웨어 설정을 완료 합니다.
**\[적용]** 메뉴를 터치

![[그림 3.1-4 산업용 통신 설정 화면]](<../_assets/3-Settings-Industrial-Communication/3.1-Setting-Firmware/image_4.png>)

{% hint style="warning" %}
**\[주의]**

<1>. **\[적용]** 버튼을 터치하여 펌웨어 설정 완료 시 해당 슬롯에 적용 되어있는 CONFIG 파일이 모두 삭제된 후 변경됩니다. 통신 펌웨어를 변경 하실 경우 기존 설정을 별도로 보관하는 것을 권장합니다.

<2>. **\[적용]** 버튼을 터치하지 않고 **\[OK]**버튼을 터치할 경우 선택한 펌웨어가 적용되지 않습니다.
{% endhint %}

<br>

##### 4. 각 슬롯마다 2. \~ 3.번을 반복하여 펌웨어를 설정해 줍니다.

<br>

##### 5. 제어기를 재부팅하여 설정한 펌웨어를 적용합니다.
**\[서비스 > 19: 산업용 통신 모니터링]** 메뉴를 터치하여 설정한 통신이 적용 되었는지 확인합니다.

![[그림 3.1-5 산업용 통신 설정 화면]](<../_assets/3-Settings-Industrial-Communication/3.1-Setting-Firmware/image_5.png>)



{% hint style="warning" %}
**\[주의]**: 펌웨어의 설정 시 제어기를 재부팅 할 때 설정값이 시스템에 적용됩니다.
{% endhint %}
