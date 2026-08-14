## 4.3 MRP

BD671은 MRP Client로 설정하여 케이블 이중화 기능을 사용할 수 있습니다.
기본 PROFINET 설정 외에 MRP 기능을 사용하기 위해 다음과 같이 설정하십시오.

1) 토폴로지 설정
<p align="center">
<img src="../_assets/4-pnio/mrp-topology.png"></img>
<em><p align="center">Topology </p></em>
</p>

2) MRP Client 설정

<p align="center">
<img src="../_assets/4-pnio/mrp_set_client.png"></img>
<em><p align="center">MRP Client </p></em>
</p>

3) Watchdog Time 설정 (200 msec 이상 설정)

 - MRP Manager의 토폴로지 재구성을 위해 최소 200ms 이상 설정해 주어야 함(그림 참고)

<p align="center">
<img src="../_assets/4-pnio/mrp_watchdog.png"></img>
<em><p align="center">Watchdog Time </p></em>
</p>


