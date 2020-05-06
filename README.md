# Azure IoT Workshop

사전 설치 항목<BR>
 <HR>
   <ul>
<li>사용가능한 Azure Subscription</li> 
     <li>Azure Portal접속 </li>
     <li>VSCode : https://code.visualstudio.com/ </li>
     <li>Python 3.7 이상 </li>
<li>Python Sample: https://github.com/Azure-Samples/azure-iot-samples-python/archive/master.zip </li>
   </ul>
  <br>
Azure IoT Hub생성 및 시물레이션 장치를 이용한 Telemetry데이터 전송
<hr>
<ol>
<li>Azure IoT Hub생성합니다.<BR>
 다음 URL의 사이트를 참고하여 Azure IoT Hub를 생성하고 장치(MyDeviceID)를 추가합니다. 
https://docs.microsoft.com/ko-kr/azure/iot-hub/iot-hub-create-through-portal 
 </li>
 <li>
생성된 장치의 기본 연결 문자열을 복사합니다. 
 </li> 
 <li>
  VSCode에서 IoT Hub와의 연결설정을 아래 URL을 참고하여 설정합니다. <Br>
 https://docs.microsoft.com/ko-kr/azure/iot-hub/iot-hub-vscode-iot-toolkit-cloud-device-messaging
 </li>
 
 <li>
다운로드 받은 Python 예제의 SimulatedDevice.py를 VSCode에서 불러옵니다.<br>
예제 파일은 Python 프로젝트 샘플의 루트 폴더 밑에 iot-hub\Quickstarts\simulated-device 폴더에 있습니다. 
</li>
 <li>
  이전 단계에서 복사한 연결 문자열을 붙여 놓습니다. <br>
  <img src ="https://github.com/keonlee/IoTWorkshop/blob/master/contring.jpg" >
 </li>
<li>
 터미널 창에서(cmd.exe) 아래 명령줄을 실행합니다. <br> pip install azure-iot-device
 </li>
 <li>
  터미널 창에서 다음 명령을 실행하여 시뮬레이션된 디바이스 애플리케이션을 실행합니다.<br>
  python SimulatedDevice.py
  
 </li>
 <li>
 VSCode에서 메세지를 모니터링 합니다 <br>
 방법: https://docs.microsoft.com/ko-kr/azure/iot-hub/iot-hub-vscode-iot-toolkit-cloud-device-messaging#monitor-device-to-cloud-messages 
 </li>
</ol>
