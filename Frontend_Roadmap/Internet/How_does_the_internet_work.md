## 인터넷이란?

>`인터넷(Internet)` 이란 정보를 담고 있는 각 컴퓨터들을 TCP/IP 라는 통신 프로토콜을 이용해 서로 정보를 주고받도록 한 컴퓨터 네트워크를 말한다.

>인터넷은 웹의 핵심적인 기술이다. 인터넷의 가장 기본적인 것은, 컴퓨터들이 서로 통신 가능한 거대한 네트워크라는 것이다.

## 인터넷에 대해

<li>인터넷의 이름은 1973년 TCP/IP 를 적립한 사람들이 '네트워크의 네트워크' 를 구현하여, 모든 컴퓨터를 하나의 통신망에 연결 (International Network) 하고자 하는 의도에서 이를 줄여 Internet 이라 명명했다.</li> 
<br>
<li>컴퓨터가 `서버` 와 `클라이언트` 로 연결되어 TCP/IP 를 이용해 정보를 주고 받게 되었다.</li> 
<br>
<li><strong>인터넷을 최초로 사용한 곳</strong>은 미국의 국방성의 아파넷이고, 초기에는 연구목적으로 쓰였으나 참여기관이 늘면서 다양한 목적으로 아파넷을 요구하였다.</li> 
<br>
<li> PC 통신처럼 모든 서비스를 제공하는 중심이 되는 호스트 컴퓨터도 없고 관리하는 조직도 없다. 인터넷을 대표하는 조직으로 ISOC 가 있지만 인터넷을 총괄 관리하는 기구는 아니다.</li> 
<br>
<li>인터넷은 총괄적으로 관리하지는 않지만 인터넷상의 어떤 컴퓨터 또는 통신망에 이상이 발생하더라도 전체에 영향을 주지 않도록 관리와 접속은 각지에서 분산적으로 행해진다.</li> 
<br>
<li>인터넷은 하이퍼텍스트 마크업 언어(HTML)나 전자 우편을 지원하는 기반 기술 등을 통해 광대한 범위의 정보 자원과 서비스들을 운반한다.</li> 
<br>
<li>대중적인 월드 와이드 웹 <code>(World Wide Web, WWW, W3)</code>은 하이퍼텍스트 전송 프로토콜(HTTP)과 함께 사용되고, HTTP로 되어 있는 웹 페이지를 보기 위한 웹 브라우저로는 마이크로소프트의 인터넷 익스플로러, 구글이 만든 크롬을 이용한다.</li> 

<hr>

## 인터넷의 변화과정

### 1.단순한 네트워크

#### 1:1 연결

두 개의 컴퓨터가 통신이 필요할 때, 우리는 다른 컴퓨터와 물리적으로 (보통 이더넷 케이블) 또는 무선으로 (예를 들어, WiFi 나 Bluetooth 시스템) 연결되어야 한다. 모든 현대 컴퓨터들은 이러한 연결 중 하나를 이용하여 연결을 지속할 수 있다.

두 대의 컴퓨터를 연결한다고 가정했을 때, 아래와 같은 모양일 것이다.

<br>
<img src="../../img/1to1_network.png">

#### N:N 연결

네트워크는 두 대의 컴퓨터로 제한되지 않는다. 원하는 만큼의 컴퓨터를 연결할 수 있다. 그러나 이렇게 연결할 수록 매우 복잡해진다.

> ex) 10대의 컴퓨터를 연결하려는 경우 컴퓨터 당 9개의 플러그가 달린 45개의 케이블이 필요하다!

<br>
<img src="../../img/NtoN_network.png">

#### Router 연결

<strong><code>N:N연결</code></strong> 문제를 해결하기 위해 네트워크의 각 컴퓨터는 `라우터`라고하는 특수한 소형 컴퓨터에 연결된다. 이 `라우터`에는 단 하나의 작업만 있다. 철도역의 신호원처럼 주어진 컴퓨터에서 보낸 메시지가 올바른 대상 컴퓨터에 도착하는지 확인한다. 컴퓨터 B에게 메시지를 보내려면 컴퓨터 A가 메시지를 라우터로 보내야하며, `라우터`는 메시지를 컴퓨터 B로 전달하고 메시지가 컴퓨터 C로 배달되지 않도록해야한다.

> 라우터를 시스템에 추가하면 10대의 컴퓨터 네트워크에는 10개의 케이블만 필요합니다. 각 컴퓨터마다 단일 플러그와 10개의 플러그가 있는 하나의 라우터가 필요하다.

<br>
<img src="../../img/router_network.png">

### 2.네트워크 속의 네트워크

그렇다면 수 백, 수 천, 수 십억 대의 컴퓨터를 연결하려면 라우터에 그만큼의 플러그가 필요하고 모든 컴퓨터가 연결되어야 할까? 일단, 라우터 자체로도 그 정도까지 확장할 수 없다. 그렇다면 어떻게 해야할까?

앞서 라우터 또한 '컴퓨터'라고 했었다. 따라서 두 대 이상의 라우터도 연결할 수 있다. 아래 그림은 각각의 라우터로 연결된 두 개의 네트워크를 연결한 모습이다.

<br>
<img src="../../img/two_router_network.png">

>컴퓨터를 라우터에 연결하고, 라우터에서 라우터로 연결함으로써 연결을 무한히 확장할 수 있다.

<br>
<img src="../../img/router_to_router_network.png">

이러한 네트워크는 우리가 인터넷이라고 부르는 것에 매우 가깝다. 그러나 우리는 뭔가를 놓치고 있다. 우리는 우리의 목적을 가지고 네트워크를 구축했고 이제 누구든지 컴퓨터로 이루어진 그들만의 네트워크를 가질 수 있다. 하지만 아직까지 우리에게는 물리적 한계가 존재한다. 집과 다른 지역 사이에, 아주 먼 곳에 케이블을 연결할 수는 없다. 그렇다면 어떻게 이 문제를 해결해야 할까?

우리는 이미 모든 집집마다 연결된 케이블이 있다. 전화기 기반의 시설은 이미 세계 어느 곳과도 연결되어 있으므로 우리가 필요로 하는 완벽한 배선이라고 할 수 있다. 따라서 우리의 네트워크를 전화 시설과 연결하기 위해선, `모뎀`이라는 특수 장비가 필요하다. `모뎀`은 우리 네트워크의 정보를 전화 시설에서 처리 할 수있는 정보로 바꾸며, 그 반대의 경우도 마찬가지이다.

>모뎀은 우리 네트워크의 정보를 전화 시설에서 처리 할 수있는 정보로 바꾸며, 그 반대의 경우도 마찬가지이다.

<br>
<img src="../../img/router_to_modem.png">

모뎀으로 우리의 네트워크는 전화 시설에 연결된다. 다음 단계는 우리의 네트워크에서 도달하려는 네트워크로 메시지를 보내는 것이다. 메세지를 보내기 위해 네트워크를 인터넷 서비스 제공 업체 (Internet Service Provider, ISP)에 연결한다.

>ISP는 모두 함께 연결되는 몇몇 특수한 라우터를 관리하고 다른 ISP의 라우터에도 액세스 할 수 있는 회사이다. 따라서 우리 네트워크의 메시지는 ISP 네트워크의 네트워크를 통해 대상 네트워크로 전달된다. 인터넷은 이러한 전체 네트워크 인프라로 구성된다.

<hr>

### 참고
<a href="https://ko.wikipedia.org/wiki/%EC%9D%B8%ED%84%B0%EB%84%B7">인터넷 [위키백과]</a>

<a href="https://developer.mozilla.org/ko/docs/Learn/Common_questions/How_does_the_Internet_work#%EC%BB%B4%ED%93%A8%ED%84%B0_%EC%B0%BE%EA%B8%B0">인터넷은 어떻게 동작하는가? [MDN]</a>

<br>
<br>
<br>