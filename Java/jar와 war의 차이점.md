# Jar 와 War 의 차이점


JAR(Java Archive)와 WAR(Web Application Archive)는 Java 기반 애플리케이션을 패키징하기 위한 파일 포맷
- 사용 목적과 포함된 내용에서 차이가 있습니다.

### 주요 차이점

| **구분**       | **JAR**                                                                 | **WAR**                                                                 |
|----------------|-------------------------------------------------------------------------|-------------------------------------------------------------------------|
| **정의**       | 일반 Java 애플리케이션 또는 라이브러리를 패키징한 파일.                   | 웹 애플리케이션을 패키징한 파일.                                        |
| **포함 내용**  | Java 클래스 파일, 메타데이터, 리소스 파일 등.                              | JSP, 서블릿, HTML, CSS, JavaScript 등 웹 애플리케이션 관련 자원 포함.     |
| **구조**       | 자유로운 구조.                                                           | `WEB-INF`, `META-INF` 등 사전 정의된 디렉토리 구조 필요.                |
| **실행 환경**  | **JRE(Java Runtime Environment)만 있으면 실행 가능.**                         | **Tomcat, WebLogic 등 웹 서버(WEB) 또는 WAS(Web Application Server) 필요.** |
| **목적**       | 독립 실행형 애플리케이션 또는 라이브러리 배포.                             | 웹 애플리케이션 배포 및 실행.                                           |

### 활용 사례
- **JAR**: 스탠드얼론 Java 애플리케이션, 재사용 가능한 라이브러리, 의존성 패키지
- **WAR**: Java 기반의 웹 애플리케이션 서버에서 실행되는 프로젝트

### 선택 기준
- **JAR**는 간단한 독립형 서비스나 마이크로서비스 아키텍처에 적합함
- **WAR**는 복잡한 대규모 웹 애플리케이션에서 서버의 고급 기능(예: 세션 관리)을 활용할 때 유용함

