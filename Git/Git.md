# Git?

Linux 를만든 '리누스 토발즈'가 개발한
**`분산형 버전관리 시스템`**

## 버전관리?
- 파일변화를 시간에 따라 기록했다가 나중에 특정 시점의 버전을 다시 꺼내올 수 있는 시스템. **VCS**라고 한다
1. 로컬 버전 관리
    - 간단한 데이터베이스를 사용해서 파일의 변경 정보 관리.
    - RCS - MAC OS X 개발 도구에 포함되어 있다.
    - Patch Set(파일에서 변경되는 부분)을 관리.
    - Patch set을 적용해 모든 파일을 특정 시점으로 되돌릴 수 있다
2. 중앙 집중식 버전 관리 CVCS협업 불가, 백업 불가
    - 중앙 데이터베이스에 문제가 생기면 프로젝트의 모든 히스토리를 잃는다.
3. 분산 버전 관리 시스템 DVCS
    - 저장소 전부를 복제.
    - 클라이언트 중 아무거나 골라도 서버를 복원할 수 있다.
    - 리모트 저장소가 존재한다.

## Git
- **거의 모든 명령을 로컬에서** 실행.
    - 프로젝트의 모든 히스토리가 로컬 디스크에 존재.
        - 명령을 신속히 실행.
        - **오프라인 상태에서도 가능**
- **check sum**으로 데이터를 관리한다.

## Git 에서 관리하는 파일의 상태
- Committed
    - 로컬 데이터베이스에 안전하게 저장됨. 
- Modified
    - 수정한 파일을 아직 로컬 데이터베이스에 커밋하지 않음.
- Staged
    - 현재 수정한 파일을 곧 커밋할 것이라는 상태.

