### 2.4.4 EtherNet/IP 스캐너 (마스터) 에러 코드

<br>

{% hint style="info" %}
\.      각 장치별 통신 상태를 CIP 표준 General Status 코드로 표시하여 실시간 진단 기능을 제공합니다.
{% endhint %}

<br>

![[그림 2.4.4-1 스캐너 설정]](<../../_assets/2-ethernet-ip/4-scanner/img_8.png>) 

<br>

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**General Status Codes**

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>상태 값 (16진수)</th>
		<th class='powderblued'>명칭</th>
		<th class='powderblued'>설명</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>-</td>
		<td>통신 설정 안됨 또는 변경됨</td>
		<td>통신 설정이 반영되지 않았거나 변경 중</td>
	</tr>
	<tr>
		<td>0x00</td>
		<td>Success</td>
		<td>서비스가 성공적으로 수행됨</td>
	</tr>
	<tr>
		<td>0x00 (에러 상태인 경우)</td>
		<td>No reponse</td>
		<td>통신 응답 없음 (케이블 연결 안됨, 유효하지 않은 IP 주소 등)</td>
	</tr>
	<tr>
		<td>0x01</td>
		<td>Connection failed</td>
		<td>연결 시도 실패 (설정 값 또는 경로 문제)</td>
	</tr>
	<tr>
		<td>0x02</td>
		<td>Resource unavailable</td>
		<td>장치 자원 부족 (연결 개수 초과 등)</td>
	</tr>
	<tr>
		<td>0x03</td>
		<td>Invalid parameter value</td>
		<td>파라미터 값 오류 (주로 데이터 크기 불일치)</td>
	</tr>
	<tr>
		<td>0x04</td>
		<td>Path segment error</td>
		<td>경로 세그먼트 오류 (Class, Instance 등 식별 불가)</td>
	</tr>
	<tr>
		<td>0x05</td>
		<td>Path destination unknown</td>
		<td>대상 객체(Object)를 찾을 수 없음</td>
	</tr>
	<tr>
		<td>0x06</td>
		<td>Partial transfer</td>
		<td>데이터의 일부만 전송됨</td>
	</tr>
	<tr>
		<td>0x07</td>
		<td>Connection lost</td>
		<td>통신 중 연결이 끊어짐 (Timeout 등)</td>
	</tr>
	<tr>
		<td>0x08</td>
		<td>Service not supported</td>
		<td>객체가 요청한 서비스(Get/Set 등)를 지원 안 함</td>
	</tr>
	<tr>
		<td>0x09</td>
		<td>Invalid attribute value</td>
		<td>설정하려는 속성값이 유효 범위를 벗어남</td>
	</tr>
	<tr>
		<td>0x0A</td>
		<td>Attribute list error</td>
		<td>속성 리스트 서비스 수행 중 오류 발생</td>
	</tr>
	<tr>
		<td>0x0B</td>
		<td>Already in requested state</td>
		<td>객체가 이미 요청한 상태에 있음</td>
	</tr>
	<tr>
		<td>0x0C</td>
		<td>Object state conflict</td>
		<td>객체의 현재 상태에서 허용되지 않는 서비스 요청</td>
	</tr>
	<tr>
		<td>0x0D</td>
		<td>Object already exists</td>
		<td>이미 존재하는 객체를 생성하려고 시도함</td>
	</tr>
	<tr>
		<td>0x0E</td>
		<td>Attribute not settable</td>
		<td>쓰기가 불가능한(Read-only) 속성에 쓰기 시도</td>
	</tr>
	<tr>
		<td>0x0F</td>
		<td>Privilege violation</td>
		<td>권한 부족 (보안이나 접근 레벨 문제)</td>
	</tr>
	<tr>
		<td>0x10</td>
		<td>Device state conflict</td>
		<td>장치의 현재 모드 또는 상태에서 요청된 서비스 실행 할 수 없음</td>
	</tr>
	<tr>
		<td>0x11</td>
		<td>Reply data too large</td>
		<td>응답 데이터가 할당된 버퍼보다 커서 전송 실패</td>
	</tr>
	<tr>
		<td>0x12</td>
		<td>Fragmentation of primitive value</td>
		<td>데이터 분할 전송 중 오류</td>
	</tr>
	<tr>
		<td>0x13</td>
		<td>Not enough data</td>
		<td>요청을 수행하기에 데이터 양이 부족함</td>
	</tr>
	<tr>
		<td>0x14</td>
		<td>Attribute not supported</td>
		<td>요청한 속성(Attribute) 번호가 존재하지 않음</td>
	</tr>
	<tr>
		<td>0x15</td>
		<td>Too much data</td>
		<td>요청에 포함된 데이터가 너무 많음</td>
	</tr>
	<tr>
		<td>0x16</td>
		<td>Object does not exist</td>
		<td>대상 객체가 존재 하지 않음</td>
	</tr>
	<tr>
		<td>0x17</td>
		<td>Service fragmentation sequence erroruccess</td>
		<td>서비스 분할 전송 순서가 잘못됨</td>
	</tr>
	<tr>
		<td>0x18</td>
		<td>No stored attribute data</td>
		<td>저장된 속성 데이터가 없음</td>
	</tr>
	<tr>
		<td>0x19</td>
		<td>Store operation failure</td>
		<td>데이터 저장 작업 실패</td>
	</tr>
	<tr>
		<td>0x1A</td>
		<td>Routing failure, request packet too large</td>
		<td>요청 데이터의 용량이 제한치를 초과하여 라우팅 서비스 중단</td>
	</tr>
	<tr>
		<td>0x1B</td>
		<td>Routing failure, response packet too large</td>
		<td>응답 데이터의 용량이 제한치를 초과하여 라우팅 서비스 중단</td>
	</tr>
	<tr>
		<td>0x1C</td>
		<td>Missing attribute list entry data</td>
		<td>요청된 동작을 수행하는데 필요한 속성이 누락됨</td>
	</tr>
	<tr>
		<td>0x1D</td>
		<td>Invalid attribute value list</td>
		<td>유효하지 않은 속성들에 대한 상태 정보 반환</td>
	</tr>
	<tr>
		<td>0x1E</td>
		<td>Embedded service error</td>
		<td>장치 내장 서비스 오류</td>
	</tr>
	<tr>
		<td>0x1F</td>
		<td>Vendor specific error</td>
		<td>장치 제조사가 직접 정의한 에러</td>
	</tr>
	<tr>
		<td>0x20</td>
		<td>Invalid parameter</td>
		<td>요청된 파라미터가 CIP 규격 또는 정의된 규격과 맞지 않음</td>
	</tr>
	<tr>
		<td>0x21</td>
		<td>Write-once value already written</td>
		<td>한 번만 쓰기 가능한 값을 이미 썼음</td>
	</tr>
	<tr>
		<td>0x22</td>
		<td>Invalid reply received</td>
		<td>잘못된 응답이 수신됨</td>
	</tr>
	<tr>
		<td>0x23</td>
		<td>Reserved</td>
		<td>-</td>
	</tr>
	<tr>
		<td>0x24</td>
		<td>Reserved</td>
		<td>-</td>
	</tr>
	<tr>
		<td>0x25</td>
		<td>Key failure in path</td>
		<td>경로 내 키(Key) 일치 확인 실패</td>
	</tr>
	<tr>
		<td>0x26</td>
		<td>Path size invalid</td>
		<td>경로 데이터 크기가 유효하지 않음</td>
	</tr>
	<tr>
		<td>0x27</td>
		<td>Unexpected attribute in list</td>
		<td>현재 상태에서 설정할 수 없는 항목 설정 시도</td>
	</tr>
	<tr>
		<td>0x28</td>
		<td>Invalid member ID</td>
		<td>지정된 클래스 / 인스턴스 또는 속성에 해당 항목이 존재하지 않음</td>
	</tr>
	<tr>
		<td>0x29</td>
		<td>Member cannot be set</td>
		<td>수정할 수 없는 항목 수정 요청</td>
	</tr>
	<tr>
		<td>0x2A</td>
		<td>Group 2 only server general failure</td>
		<td>DeviceNet Error (EtherNet/IP 에서 미사용)</td>
	</tr>
	<tr>
		<td>0x2B - 0xCF</td>
		<td>Reserved</td>
		<td>-</td>
	</tr>
	<tr>
		<td>0xD0 - 0xFF</td>
		<td>Vendor specific Codes</td>
		<td>장치 제조사가 직접 정의한 에러</td>
	</tr>
</tbody>
</table>
<br>
