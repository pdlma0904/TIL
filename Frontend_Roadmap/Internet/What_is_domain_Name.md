## 도메인 네임

도메인 네임은 인터넷 인프라의 핵심 부분이다. 인터넷에서 사용할 수있는 모든 웹 서버에 대해 사람이 읽을 수있는 주소를 제공한다.

>인터넷에 연결된 모든 컴퓨터는 IPv4의 경우 32비트로 구성되거나 IPv6의 경우 128비트로 구성된 공용 IP 주소를 통해 연결할 수 있다.
>
> - **IPv4** : 일반적으로 0과 255 사이의 4개의 숫자로 쓰여지며 점으로 구분된다.
(ex: 173.120.121.32)
> - **IPv6** : 일반적으로 4개의 16진수 숫자로 구성된 8개의 그룹으로 작성되며, 콜론으로 구분된다.
(ex: 2027:0da8:8b73:0000:8a2e:0370:1337)

컴퓨터는 이러한 주소를 쉽게 처리할 수 있지만, 사람들은 누가 서버를 실행하고 있는지 또는 웹 사이트가 제공하는 서비스를 찾기 어렵다. IP 주소는 기억하기 어렵고 시간이 지남에 따라 변경될 수 있다. 이러한 모든 문제를 해결하기 위해 도메인 이름이라고 하는 사람이 읽을 수 있는 주소를 사용한다.

## Domain name의 구조

도메인 이름은 몇개의 파트로 이루어진 간단한 구조를 이루고 있다. 점으로 구분하고 오른쪽에서 왼쪽으로 읽는다.
<img src="../../img/domain_name.png">

### TLD (Top-Level Domain; 최고레벨 도메인).
 - 가장 일반적인 정보를 제공한다.
 - TLD는 도메인 이름 뒤에 있는 서비스의 일반적인 목적을 사용자에게 알려준다.
>가장 일반적인 TLD(.com, .org, .net)는 엄격한 기준을 충족하는 웹 서비스가 필요하지 않지만 일부 TLD는 보다 엄격한 정책을 시행한다. 예를 들어 `.us`, `.fr`, `.sh`와 같은 로컬 TLD는 해당 서비스가 특정 언어로 제공되거나 특정 국가에서 호스팅되도록 요구할 수 있다.

### Label (or component)
 - 레이블은 TLD 이전에 나온다.
 - TLD 바로 앞에 있는 Label을 SLD(Secondary Level Domain)이라고도 한다.
 - 도메인 이름을 구성하기 위해 3개의 레이블을 사용하는 것은 아니다.

## 도메인 이름 구매하기
도메인 이름을 구입할 수는 없다. 엄밀히 말하자면 도메인 이름을 일정기간(1년이상)동안 빌리는 것이다. registrars라고 하는 회사는 도메인 이름 저장소 사용하여 사용자를 도메인 이름에 연결해준다.

### 이용가능한 Domain Name 찾기
- domain name을 판매하는 registar의 웹 사이트에 들어가서 확인하기
- shell이 내장된 시스템을 사용하는 경우 whois 명령어를 사용하여 확인하기