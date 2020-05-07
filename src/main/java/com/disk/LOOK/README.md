# LOOK Disk Scheduling

* Language : Java
* IDE : Intellij IDA
* 날짜 : 20.05.06

## Description

LOOK 스케줄링은 SSTF와 같은 방식의 운영이지만, 차이점이 있다. 현재 진행 방향상의 짧은 거리에 있는 요청을 서비스하는 기법인 점이다.  SCAN 알고리즘과 유사한데, SCAN은 헤드의 각 방향에 트랙 끝까지 이동하고, LOOK은 마지막 트랙까지만 이동한다. 

LOOK 알고리즘은 엘리베이터 알고리즘이라고도 한다.  실제 엘리베이터 알고리즘이 이렇게 동작한다. 

SSTF의 단점인 기근 현상을 보완하기 위하여 나온 모델로, 디스크 스케줄링의 기본 모델로 쓰이고 있다.

<img src="/doc/disk/LOOK/LOOK.png">

<br>

### LOOK 특징

---
1. 여전히 사이드와 중앙 간의 서비스 편차가 존재
2. SSTF보다 효율적
3. 현재 진행 방향에 더이상의 요청이 없을 때 방향이 바뀐다. <br>
( 따라서, 그 사이에 반대 라인에 생기는 요청은 오랫동안 대기하게 됨)
---