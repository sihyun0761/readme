동아리 활동 중 제슨나노 프로젝트를 진행함. 먼저, SD카드에 Balena Etcher를 사용해 우분투 이미지를 구웠음. Balena Etcher는 다양한 운영체제 이미지를 SD카드나 USB에 쉽게 설치할 수 있는 도구로, 설치 과정에서 오류 발생 가능성이 낮음. 이후 SD카드를 제슨나노에 꽂고, 무선 인터넷 연결을 위해 USB 와이파이 동글을 사용해 와이파이 설정 완료. 제슨나노는 기본적으로 유선 이더넷만 지원하지만, 와이파이 동글을 사용하면 무선 환경에서도 사용할 수 있음. 이후 마우스, 키보드, 모니터를 연결해 제슨나노를 완전한 컴퓨터로 구성함. 이 과정에서 제슨나노의 작은 크기와 적은 소비 전력 덕분에 소형 컴퓨터로서의 장점을 체험함.

다음으로, 제슨나노의 발열 문제를 해결하기 위해 쿨링팬을 설치했음. 코딩을 통해 쿨링팬의 동작을 제어하고 속도를 조절하는 기능을 구현함. 이를 통해 제슨나노의 성능을 최대한 끌어올리는 동시에, 과열로 인한 시스템 불안정을 방지함. 이후 교육 과정에 필요한 디렉토리 구조를 설정하고, Docker를 설치해 필요한 개발 환경을 구축함. Docker는 컨테이너 기반의 가상화 도구로, 다양한 개발 환경을 손쉽게 배포하고 관리할 수 있는 장점이 있음.

데이터 크롤링 프로젝트에서는 웹에서 원하는 사진 데이터를 자동으로 수집하는 프로그램을 개발함. 이를 통해 농작물인 감자, 고구마뿐만 아니라 아이돌 멤버 수지, 카리나의 사진도 손쉽게 수집함. 데이터 크롤링은 웹에서 데이터를 자동으로 가져오는 기술로, 여기서는 파이썬의 Selenium과 BeautifulSoup 라이브러리를 활용함. Selenium은 웹 브라우저를 자동으로 제어하는 도구로, 크롬 브라우저를 통해 원하는 페이지를 열고, 특정 키워드를 입력해 검색 결과에서 사진을 다운로드함. BeautifulSoup은 HTML을 파싱해 원하는 데이터를 추출하는 데 사용됨. 크롤링 과정은 크롬 설치, 크롤링 프로그램 다운로드, 필요한 파이썬 패키지 설치, 다운로드할 키워드 입력, 크롤링 실행, 결과 확인, 데이터 정제의 단계로 진행됨. 데이터 정제는 수집된 사진이 원하지 않는 중복 키워드를 포함하거나, 불필요한 이미지가 포함된 경우 이를 걸러내는 과정임. 여기서 single-label classification 방식을 사용해 각 사진이 하나의 클래스에만 속하도록 하고, 나머지 데이터는 삭제함.

파이썬 학습에서는 기본적인 프로그래밍 개념과 실습을 진행함. Python Tutorial 사이트에서 데이터를 처리하는 다양한 방법을 학습했음. 파이썬에서는 데이터를 효율적으로 관리하고 처리할 수 있는 여러 가지 방법이 있으며, 이 과정에서 변수와 함수의 선언, 활용 방법을 익힘. 예를 들어, 문자열에서 특정 위치의 문자를 삭제하거나, 그 위치에 있는 문자를 추출하는 프로그램을 작성해 봄. 또한, 파이썬으로 파일을 생성하거나 삭제하고, 파일의 이름을 변경하는 방법도 학습함. 이를 통해 파일 시스템을 관리하는 기초적인 방법을 익혔음.

한편, 제슨나노에서 파이썬 3.6만 지원하지만, 우리가 필요한 작업은 파이썬 3.8이 필요했음. 제슨나노의 리눅스 환경에서 필요한 파이썬 버전을 설치하고 관리하는 방법을 연구하고, 여러 가지 해결 방안을 모색함. 이를 통해 제슨나노에서 더 최신 버전의 파이썬을 사용하여 작업을 진행할 수 있도록 설정함.

추가적으로, 네트워크 다운로드 도구인 `wget`의 사용법을 익힘. `wget`은 터미널에서 명령어로 파일을 다운로드할 수 있는 도구로, 특히 대용량 파일이나 여러 파일을 자동으로 다운로드할 때 유용함. 그리고 리눅스 파일 시스템에서의 파일 및 디렉토리 권한 관리에 대해 학습함. `sudo chmod 755` 명령어를 사용해 파일이나 디렉토리의 권한을 변경함. 여기서 `chmod`는 권한을 변경하는 명령어로, `755`는 파일 소유자에게 읽기, 쓰기, 실행 권한을 부여하고, 그룹과 기타 사용자에게는 읽기와 실행 권한만을 부여하는 설정임. `sudo`는 관리자 권한으로 명령을 실행하기 위한 명령어로, 이를 통해 파일 시스템의 권한을 적절히 관리함.
