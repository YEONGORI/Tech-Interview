### 로드 밸런서에 대해서 알고 계신가요?
로드 밸런서는 서버의 부하를 분산하기 위한 장치입니다. Layer 4 로드 밸런서와 Layer 7 로드 밸런서가 주로 사용되는 것으로 알고 있습니다.

### Layer4 로드 밸런서와 Layer7 로드 밸런서의 차이를 알고 계신가요?
Layer4 로드 밸런서는 MAC 주소와 IP 주소 그리고 패킷을 사용해 로드 밸런싱하고, Layer7는 Layer4에 더해서 HTTP 헤더를 사용해 로드 밸런싱합니다.

### Layer7은 어떻게 MAC주소와 IP주소 그리고 패킷의 정보를 사용할 수 있나요?
패킷헤더에 하위 계층의 정보가 담겨있기 때문입니다.

### 패킷 헤더에 대해서 설명해주실 수 있나요?
패킷의 내용과 수신 대상에 대한 정보를 담고 있는 상자입니다.

### 로드 밸런싱이 어떻게 이루어지는지도 아시는대로 설명해주세요.
다수의 서버에 순서대로 요청을 할당하는 방식과 가장 처리속도가 빠른 서버에 우선 할당하는 방식 등이 있고, 제 프로젝트에 적용된 로드 밸런싱 알고리즘은 라운드 로빈 방식으로 알고 있습니다.

### 왜 라운드 로빈 방식을 사용하셨나요?
우선 두 서버의 성능이 동일하고 아직 트래픽이 많이 발생하지 않아서 로드 밸런싱을 최적화할 필요를 느끼지 못했기 때문에 기본 설정으로 선택하였습니다.