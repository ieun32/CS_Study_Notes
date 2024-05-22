# AWS란?

`AWS`는 아마존 웹 서비스(*Amazon web services*)의 약자로, 클라우드 컴퓨팅 분야에서 압도적으로 세계 1위의 점유율을 차지하고 있는 **아마존 닷컴의 클라우드 컴퓨팅 서비스**이다.

전 세계에 분포되어 있는 데이터 센터를 통해 다양한 기능을 제공하는 클라우드 플랫폼이라고 보면 된다. 

AWS에서는 190개 이상의 서비스를 제공하고 있는데, 컴퓨팅, 스토리지, 데이터 베이스와 같은 인프라 기술부터 기계 학습 및 인공 지능, 데이터 레이크 분석, 사물 인터넷 등의 새로운 기술까지 다른 클라우드에서는 제공하지 않는 기능까지 포함하고 있으며 끊임없이 새로운 서비스가 출시되고 있다.

# 클라우드 컴퓨팅이란?

**클라우드 컴퓨팅**은 간단히 말해 컴퓨터를 빌려주는, 컴퓨터 임대 사업을 말한다. 오래된 표현으로는 호스팅 비즈니스라고 하는데, 호스트는 컴퓨터 한 개를 뜻한다.

자세히는, 서로 다른 물리적 위치에 존재하는 컴퓨터들의 자원(서버, 플랫폼, 소프트웨어 등)을 가상화 기술로 통합해 제공하는 기술을 말한다.

클라우드 컴퓨팅 서비스를 제공하는 `AWS`를 예로 들면, 다양한 기능이 있지만 본질적으로 컴퓨터를 빌려주는 서비스로 `EC2`라는 서비스가 있다. `EC2`는 *Elastic Compute Cloud* (탄력적 컴퓨팅 클라우드) 라는 뜻으로, 0.5GB의 메모리를 가진 초소형 컴퓨터를 빌릴 수 있다. 컴퓨팅 파워가 더 필요하다면 더 비싼 컴퓨터를 임대할 수도 있다.

요즘에는 컴퓨터 임대 뿐만 아니라 소프트웨어 대신 설치해주고 대신 운영해주는 방향으로 클라우드 비즈니스가  확장되고 있다. 왜냐하면 WEB, AI, Big Data, IOT 등 다양한 분야에서 서버 컴퓨터를 필요로 하는 요구 사항이 반영되어 이를 위한 서비스들이 클라우드 컴퓨팅 서비스에 계속 추가되고 있기 때문이다.

# IaaS, PaaS, SaaS란?

클라우드 컴퓨팅 서비스가 등장하기 전에는 어떤 서비스를 만들기 위해서 서비스 개발에 필요한 모든 IT 인프라 자원을 직접 구축하는 것이 일반적이었다. 예를 들어 물리적 장비, 구축, OS 및 기타 구동 프로그램 구입 및 설치, Data 보안 관리, 애플리케이션 프로그램 구입 및 설치까지 모든 과정을 직접 진행해야했다. 이러한 운영 방식을 `*On-Premise*`(온프레미스) 방식이라고 한다.

그러나 온프레미스 방식은 다음과 같은 단점이 있었다. ([출처](https://www.google.com/search?q=%EC%98%A8%ED%94%84%EB%A0%88%EB%AF%B8%EC%8A%A4+%ED%95%9C%EA%B3%84&sca_esv=ee9179209f9cefc8&ei=CqVNZu-HEsmKvr0P2I-MgAI&udm=&ved=0ahUKEwjvtMGc5KCGAxVJha8BHdgHAyAQ4dUDCBA&uact=5&oq=%EC%98%A8%ED%94%84%EB%A0%88%EB%AF%B8%EC%8A%A4+%ED%95%9C%EA%B3%84&gs_lp=Egxnd3Mtd2l6LXNlcnAiFuyYqO2UhOugiOuvuOyKpCDtlZzqs4QyBRAhGKABMgUQIRigAUiuCFCCA1iXB3ABeAGQAQCYAZEBoAHkBqoBAzAuN7gBA8gBAPgBAZgCBqACgAXCAgoQABiwAxjWBBhHwgILEAAYgAQYsQMYgwHCAgUQABiABJgDAIgGAZAGCpIHAzEuNaAHkh0&sclient=gws-wiz-serp))

- 높은 하드웨어 비용 및 감가상각
- 제한된 탄력적 운영 (물 들어올 때 인프라 확 넓혔는데, 이후에는 싹 빠져서 파리 꼬이는)
- 기업이 오류 및 보안 사고에 대해 전적으로 책임져야함
- 최첨단 기능에 대한 낮은 액세스
- 지원 종료 및 교체로 인한 문제

따라서 이러한 한계를 보완하고자 하는 요구 사항과 기술적 성장으로 클라우드 컴퓨팅이 생겨난 것이다.

한편 이러한 클라우드 컴퓨팅 서비스는 크게 `IaaS`, `PaaS`, `SaaS`의 3가지로 구분할 수 있다.

![[https://www.dknyou.com/blog/?idx=14931168&bmode=view](https://www.dknyou.com/blog/?idx=14931168&bmode=view)](./assets/images_aws/Untitled.png)

[https://www.dknyou.com/blog/?idx=14931168&bmode=view](https://www.dknyou.com/blog/?idx=14931168&bmode=view)

서비스의 종류에 따라 서비스의 영역이 달라지는데, 하나씩 살펴보도록 하자.

## IaaS (Infrastructure as a service)

![[https://www.dknyou.com/blog/?idx=14931168&bmode=view](https://www.dknyou.com/blog/?idx=14931168&bmode=view)](./assets/images_aws/Untitled%201.png)

[https://www.dknyou.com/blog/?idx=14931168&bmode=view](https://www.dknyou.com/blog/?idx=14931168&bmode=view)

`IaaS`는 **인프라를 구독형 서비스로 제공하는 클라우드 컴퓨팅 서비스**를 말한다.

보통 인프라라고 하면 철도, 지하철 등을 지칭하는데, IT에서 인프라라고 하면 **서버, 스토리지, 네트워크 장비 등의 자원**을 의미한다. 위 그림과 같이 IaaS는 네트워크부터 가상화까지 서비스를 제공한다.

컴퓨터를 예로 들면 아무 프로그램도 설치되지 않은 순수 하드웨어로서의 컴퓨터를 임대하는 것과 같다. 고객은 이 컴퓨터에 OS를 깔고, MS Office, 게임 등 필요한 소프트웨어를 설치해서 사용하게 된다.

### IaaS 예시

- AWS
- Microsoft Azure
- Google Cloud와 같은 퍼블릭 클라우드 공급 업체

## PaaS (platform as a service)



![[https://www.dknyou.com/blog/?idx=14931168&bmode=view](https://www.dknyou.com/blog/?idx=14931168&bmode=view)](./assets/images_aws/Untitled%202.png)

[https://www.dknyou.com/blog/?idx=14931168&bmode=view](https://www.dknyou.com/blog/?idx=14931168&bmode=view)

`PaaS`는 **플랫폼을 구독형 서비스로 제공하는 클라우드 컴퓨팅 서비스**를 말한다.

PaaS는 **애플리케이션 구축, 실행 및 애플리케이션 개발 환경 플랫폼을 제공하는 목적**이 있기 때문에 개발에 필요한 라이브러리, 개발 도구, 데이터 베이스, 보안 기능 등이 플랫폼에 포함된다.

컴퓨터로 예를 들면 OS 및 통신 소프트웨어 등 컴퓨터가 작동하는데 필요한 기본적인 프로그램이 설치된 컴퓨터를 임대하는 것으로 볼 수 있다. 고객은 이 컴퓨터에 필요로 하는 또는 비즈니스로 서비스 하고자 하는 애플리케이션 등을 설치해 필요한 업무 또는 서비스를 시작하면 된다. 

혹은 개발이 목적이라면 개발을 위해 준비된 환경에서 바로 개발을 시작할 수 있다. 따라서 비용 절감과 개발 주기가 단축 효과를 볼 수 있다.

PaaS에서는 소프트웨어 업데이트 또는 하드웨어 유지 관리는 모두 플랫폼이 제공하기 때문에 서비스 외적인 부분에 신경 쓸 필요가 없다.

### PaaS 예시

- AWS Elastic BeanStalk
- Heroku
- Red Hat OpenShift 등

## SaaS (software as a service)



![Untitled](./assets/images_aws/Untitled%203.png)

`SaaS`는 **소프트웨어를 구독형 서비스로 제공하는 클라우드 컴퓨팅 서비스**를 말한다.

위 그림에서 보는 것과 같이 네트워크부터 애플리케이션까지 모든 레벨을 제공 업체에서 관리한다. 즉 사용자가 곧바로 필요로 하는 업무 또는 서비스가 가능한 완비된 형태의 서비스를 가상화로 제공한다. 대부분의 SaaS 애플리케이션은 웹 브라우저를 통해 직접 실행되므로 사용자는 아무런 설치, 구축을 할 필요 없이 클라우드에서 응용 프로그램을 제공받아 사용하면 된다.

컴퓨터 리소스의 제한 없이 언제 어디서나 브라우저를 통해 접속만 하면 서비스를 사용할 수 있고, 최신 SW 업데이트를 빠르게 제공 받을 수 있다.

요즘에는 대부분의 오피스 프로그램들이 SaaS로 많이 사용되고 있다. 

### SaaS 예시

- ZOOM
- Netflix
- Google Docs
- Microsoft Office 365

# AWS EC2란?



- `EC2`는 *Elastic Compute Cloud* (탄력적 컴퓨팅 클라우드)의 약자로, 안전하고 크기 조정이 가능한 컴퓨팅 파워를 클라우드에서 제공하는 웹 서비스이다.
- `EC2`에서 컴퓨터 단위는 인스턴스이다.
    - 1 컴퓨터 = 1 인스턴스라고 부른다.

## EC2 실습

### 1. EC2 인스턴스 만들고 접속해보기

- 콘솔 로그인 하기 > 서비스 > EC2 > 인스턴스 만들기
- 프리티어 사용 가능한 윈도우 서버 선택
    
    ![Untitled](./assets/images_aws/Untitled%204.png)
    
- 인스턴스 중에 프리티어 사용 가능한 t2.micro 버전 선택
    
    ![Untitled](./assets/images_aws/Untitled%205.png)
    
- 우하단 인스턴스 생성 버튼 클릭
- 새 키 페어 생성하기 (비밀번호)
    - 그리고 인스턴스 생성 버튼을 누르면 자동으로 키가 다운되고 (잃어버림 안된다)
    - 인스턴스가 생성된다
    
    ![Untitled](./assets/images_aws/Untitled%206.png)
    
- 인스턴스에 연결 버튼 클릭
- RDP 클라이언트 > 원격 데스크톱 파일 다운로드
    
    ![Untitled](./assets/images_aws/Untitled%207.png)
    
- 암호 가져오기 > 아까 다운받은 암호 파일 업로드 > 암호 해독 > 해독된 암호 복사
- 맥에서는 별도의 프로그램 사용해서 접속해야 하고, 윈도우에서는 원격 데스크톱 다운로드 받은 파일 실행 > 해독 비밀번호 입력 > 예  눌러주면 바로 접속 가능하다.
    
    ![Untitled](./assets/images_aws/Untitled%208.png)
    

- 요금 관리하기 > 필요 없으면 중지 or 종료
    - 중지 > 전원 끄기 (데이터 보존, 전기세 나감)
        - 주의: 중지했다가 다시 시작하면 항상 다른 IP가 할당됨
    - 종료 > 컴퓨터 버리기 (데이터 삭제)
- 과금 정보 > 내 계정에 결제 탭 들어가서 확인
    - Budget: 예산 정할 수 있음, 예산 초과하는 경우 이메일 갈 수 있도록
    - 그리고 과금 안될려면 계정 삭제가 가장 좋음
        - 계정 삭제하면 90일 내에 다시 살릴 수 있고 이메일 다시 못쓴다 등등

### 2. 보안 관리: IAM 설정하기

- 사용자 권한 관리 > IAM > 대시보드

![Untitled](./assets/images_aws/Untitled%209.png)

- 주황색은 권장하는 조치, 다 초록색으로 만드는 것이 좋다
- MFA 설정하기
    - 로그인 할 때 OTP를 사용해서 한번 더 보안 절차를 거치도록 할 수 있다.
    - Multi Factor = Login+ OTP
    - 모바일 디바이스에 google authenticator 설치하고 IAM에 가상 MFA 디바이스 추가 단계를 따르면 설정이 완료된다.
    
    ![Untitled](./assets/images_aws/Untitled%2010.png)
    
    - 그러면 아래처럼 멀티 팩터 인증에 내 디바이스가 추가된다.
    
    ![Untitled](./assets/images_aws/Untitled%2011.png)
    
- 이제 로그인 할 때 OTP인증을 추가로 해야 로그인 가능하다.
    
    ![Untitled](./assets/images_aws/Untitled%2012.png)
    

# AWS S3란?



*`AWS S3`는 Simple Storage Service*의 약어로, 간단한 저장 서비스로 번역할 수 있겠다.

`AWS`를 하나의 컴퓨터로 비유했을 때, `S3`는 그 컴퓨터에 해당하는 하드디스크, SSD와 같은 저장 장치에 비유할 수 있다. 즉 **S3는 파일을 보관해주는 서비스**라고 할 수 있다.

## AWS S3 이점

### 내구성

절대 잃어버리면 안되는 파일이 있다고 하였을 때, 컴퓨터는 언제든지 고장 날 수 있으므로 파일을 잃어버리지 않는다는 보장이 없다.

이때 AWS S3를 활용하면 파일을 안전하게 보관할 수 있다. S3에 파일을 보관하게 되면 하나의 컴퓨터에만 저장되는 것이 아니고, 최소 3개 이상의 여러 대의 컴퓨터에 복사해 저장한다.

그리고 각각의 컴퓨터들은 같은 건물에 존재하지 않고 멀리 떨어져 있는 서로 다른 건물에 존재하고 있다. 따라서 한 건물이 파괴되어도 나머지 건물은 생존해 있을 가능성이 높다.

### 접근성

또한 AWS S3는 인터넷에 연결되어 있기 때문에 전 세계 누구나 업로드 되어있는 파일에 접속해서 해당 파일을 다운로드 받을 수 있다.

즉 AWS S3를 일종의 파일 서버로도 활용할 수 있다.

S3를 파일 서버로 활용하게 되면 아무리 많은 사용자가 들어와도 죽지 않는 서버로서 운영이 가능하다. 많은 사용자를 어떻게 지탱하고, 어떻게 감당할 것인지는 AWS에서 알아서 서비스로 제공해주는 부분이다.

### 자동화

어떤 파일을 저장할 때 예를 들면 5년 뒤에는 삭제되었으면 좋겠다던가, 해당 파일이 1년 뒤에는 좀 더 저렴한 저장 장치로 이동되었으면 좋겠다던가하는 요구 사항을 자동화 해주는 기능이 있다.

### 버전 관리

어떤 파일을 계속해서 수정한다고 가정할 때, 예전의 파일은 같은 이름이니 잃어버리겠지만, 이럴 때 예전에 있었던 파일을 잃어버리지 않고 자동으로 예전 버전들도 유지하고 쉽게 찾을 수 있도록 하는 기능도 제공하고 있다.

이외에도 S3에서는 수많은 유용한 기능들을 제공한다.

## S3의 구성요소

S3의 구성요소는 다음과 같다.

- `**버킷**`: 하나의 프로젝트 단위
- `**폴더**`: 하나의 폴더 단위
- `**오브젝트**`: 파일 + 메타데이터

각 구성 요소는 버킷 > 폴더 > 오브젝트 순서의 계층 관계를 갖는다.

S3에서는 이러한 오브젝트, 폴더, 버킷을 생성, 조회, 수정, 삭제(CRUD)할 수 있다.

## S3 실습

### 1. 버킷 생성

1. [**Amazon S3](https://ap-northeast-2.console.aws.amazon.com/s3/get-started?region=ap-northeast-2) > [버킷](https://ap-northeast-2.console.aws.amazon.com/s3/buckets?region=ap-northeast-2) > 버킷 만들기 조회**

![Untitled](./assets/images_aws/Untitled%2013.png)

- 버킷 이름은 전세계에서 유일한 버킷 이름을 생성해야 한다.

1. 나머지 선택 속성 중 원하는 속성을 설정한다.
    - 태그: 과금이 될 때 해당 태그 네임을 참고
    - 암호화: 서버 측에서 파일을 열람하게 된다고 할 때 암호 입력
    - 버전 관리: 파일을 수정하고 업데이트하면서 자동 파일 버전 기록
    - 퍼블릭 액세스: 누구나 파일에 접근할 수 있는 지 여부
        - 공개 파일을 올릴 수 있는 지 여부를 설정

1. 버킷 만들기 버튼을 클릭해 버킷을 생성한다.
    
    ![생성 완료된 버킷](./assets/images_aws/Untitled%2014.png)
    
    생성 완료된 버킷
    
2. 생성된 버킷을 조회한다. 버킷 이름을 클릭해 조회할 수 있고, 최초 설정은 버킷의 설정 탭에서 얼마든지 변경할 수 있다.
    
    ![Untitled](./assets/images_aws/Untitled%2015.png)
    

### 2. 폴더 생성

1. 버킷 조회 > 폴더 만들기 버튼 클릭
2. 폴더 이름 지정 > 폴더 만들기 버튼 클릭
    
    ![생성된 폴더](./assets/images_aws/Untitled%2016.png)
    
    생성된 폴더
    

### 3. 객체 생성

1. 해당 폴더 > 파일 업로드 버튼 클릭
2. 업로드 파일 선택 > 파일 업로드 버튼 클릭
    
    ![Untitled](./assets/images_aws/Untitled%2017.png)
    

### 4. 공유와 권한

1. 기본적으로 S3에 업로드 한 파일의 URL로 접속을 하면 AccessDenied 에러가 뜬다.
- S3 업로드 파일의 URL 정보 확인
    
    ![Untitled](./assets/images_aws/Untitled%2018.png)
    
- URL로 접속 후 뜨는 AccessDenied Error
    
    ![Untitled](./assets/images_aws/Untitled%2019.png)
    

1. 누구나 해당 파일에 접근할 수 있게 하기 위해서는 파일 > 권한 탭에서 설정을 변경해줘야 한다.
- 먼저 버킷의 ACL 설정과, 퍼블릭 액세스 차단 설정을 변경해주어야 한다.
    
    ![버킷 > 권한 > 객체 소유권 편집 > ACL 활성화 > 변경 사항 저장](./assets/images_aws/Untitled%2020.png)
    
    버킷 > 권한 > 객체 소유권 편집 > ACL 활성화 > 변경 사항 저장
    
    ![버킷 > 권한 > 퍼블릭 액세스 차단 설정 변경 (체크 해제 참고) > 변경 사항 저장](./assets/images_aws/Untitled%2021.png)
    
    버킷 > 권한 > 퍼블릭 액세스 차단 설정 변경 (체크 해제 참고) > 변경 사항 저장
    

1. 설정을 마친 뒤 파일 > 권한 탭에서 전체 공개 설정을 할 수 있다.
    
    ![파일 > 권한 탭](./assets/images_aws/Untitled%2022.png)
    
    파일 > 권한 탭
    
    - 피부여자 종류
        - 객체 소유자: 내가 가진 권한을 의미
        - 모든 사람: 말 그대로 모든 사람을 의미
        - 인증된 사용자 그룹: 말 그대로 인증된 사용자 그룹을 의미
    - 권한 > 편집 버튼 클릭 > 전체 공개 체크 > 변경 사항 저장
        
        ![Untitled](./assets/images_aws/Untitled%2023.png)
        

1. 다시 주소로 접근해보기
- 이제는 전체 공개가 되어 주소로 접근하면 해당 텍스트 파일을 조회할 수 있다.

![Untitled](./assets/images_aws/Untitled%2024.png)

### 5. 스토리지 클래스

스토리지 클래스는 다음과 같은 종류가 있다.

파일마다 스토리지 클래스를 설정할 수 있다. 파일의 수준을 설정할 수 있다.

![Untitled](./assets/images_aws/Untitled%2025.png)

- 가용 영역은 이 파일이 최소 몇 개의 컴퓨터에 저장될 것인지 여부

### 6. 요금체계

요금 체계는 스토리지 클래스 별로, 사용하고 있는 저장 용량 별로, 네트워크 사용량 별로 정책이 나뉘어져 있다.

요금 체계는 [여기서](https://aws.amazon.com/ko/s3/pricing/?nc=sn&loc=4) 확인할 수 있다.

![Untitled](./assets/images_aws/Untitled%2026.png)

## S3 파일 보관 이외 기능

S3에는 파일 보관 기능 말고도 다양한 기능을 제공한다.

- **정적 웹 사이트 호스팅**
    - 정적 웹사이트 호스팅을 사용하면 S3에 보관한 파일로 전세계 누구나 방문할 수 있는 웹사이트를 만들 수 있다.
- **Cloud Front**
    - 만약 서울에 region을 갖고 있는 파일을 뉴욕으로 서빙하면 오랜 시간이 걸려, 뉴욕에 주 고객이 있다면 고객 이탈로 이어질 수 있다. 따라서 S3는 Cloud Front 기능을 제공한다.
    - 이런 서비스를 Content Delivery Network (CDN)라고 부르며, 전세계에 CDN 서버를 분리해두었다가, 요청이 들어오면 가장 가까운 서버에 미리 저장하고 있었던 콘텐츠를 보내주는 원리이다.
- **버전 관리**
    - S3는 버전 관리 기능을 자체적으로 가지고 있다.
    - 같은 이름의 파일을 변경하면 변경된 내용을 모두 보관한다.
- **Life cycle**
    - 시간이 지남에 따라 조회가 줄어드는 파일 유형이 있다. 가령 SNS에 올리는 사진 파일은 올린 날 당일에는 조회수가 많겠지만 1년이 지났을 경우 조회수가 많이 줄어들 것이다.
    - 따라서 처음에 업로드 되었을 때는 스탠다드 클래스를 사용하다가 한 달이 지나면 standard-ia (infrequent access) 클래스로 변경하는 작업을 자동화 할 수 있다.
    

# AWS CloudFront란?



클라우드 프론트 서비스에서는 대표적으로 아래 두 가지 서비스를 제공한다.

서비스를 이해하기 위해서는 두 가지에 대한 이해가 필요하다.

- `Cache Server` + `CDN`
- 클라우드 프론트는 기본적으로 캐시 서버인 동시에, 전 세계에 흩어져 있는 AWS 인프라를 이용하는 캐시 서버이기 때문에 CDN으로서 동작하기도 한다.

## Cache Server

- Node.js나 php로 웹페이지를 만들어서 서비스하고 있다면, 요청이 있을 때마다 html 파일을 생성해서 보내주는 방식으로 웹페이지를 서빙할 것이다.
- 만약 페이지의 변경이 적다면 이러한 방식은 매우 비효율적이라고 할 수 있다.
- 이때 매번 요청을 하는 것이 아니라 페이지를 한 번만 요청하고 이후에는 저장된 결과를 서비스 할 수 있다면 효율적인 서비스가 가능할 것이다.
- 이처럼 저장된 결과를 이용해서 응답하는 것을 ‘저장’이라는 의미에서 캐시라고 부른다.
    - Cache: 저장하다 (v)
- 이러한 캐싱을 전담하는 서버를 캐싱 서버라고 한다.
- 클라우드 프론트의 첫번째 기능은 바로 이 **캐싱 서버로서의 역할을 제공**하는 것이다.

## CDN: Content Delivery Network

- 웹 서비스를 운영하는데, 서버가 서울에 있다고 가정하자.
- 만약 주 고객이 뉴욕, 런던, 케이프 타운에 있고 해당 지역에서 서버에 접속하는데 5초, 많게는 10초 이상 걸린다면 고객이 이탈하게 될 것이다.
- 따라서 이러한 상황을 극복하기 위해 전세계에 서버를 분리해두었다가, 요청이 들어오면 가장 가까운 서버에 미리 저장하고 있었던 콘텐츠를 보내주는 방법을 사용할 수 있다.
- 이러한 방법을 CDN이라고 하고, 클라우드 프론트의 두번째 기능이 바로 **CDN을 제공**하는 것이다.

따라서 이러한 클라우드 프론트를 활용하면 웹서버의 부담을 경감시키고,

전세계 사용자를 대상으로 고속으로 컨텐츠를 제공할 수 있다.

## 클라우드 프론트 실습

### 1. PHP 웹 어플리케이션 생성

- 여기 다음과 같이 문자열과 현재 날짜를 출력하는 PHP 어플리케이션을 만들고, CDN 성능을 확인해보기 위해 PHP 문법을 사용해서 로딩 시간을 1초 늦춰보자. 그리고 웹 서버를 사용해서 웹 어플리케이션을 서빙해보자.

![로딩에 1.4초가 걸리는 웹 애플리케이션](./assets/images_aws/Untitled%2027.png)

로딩에 1.4초가 걸리는 웹 애플리케이션

### 2. 클라우드 프론트 생성

- 네트워크 & 콘텐츠 딜리버리 > CloudFront 서비스 > Create Distribution 버튼 클릭
    
    ![Untitled](./assets/images_aws/Untitled%2028.png)
    
- 클라우드 프론트를 사용하게 되면 사용자는 더 이상 웹 서버로 직접 접속하지 않는다. 최초 요청 시 클라우드 프론트가 웹 서버에게 웹페이지를 요청하면, 웹 서버가 전달해주고, 이후 요청 부터는 클라우드 프론트가 그 결과를 저장하고 있다가 사용자에게 전달한다. 즉 최초 요청 이후부터는 웹서버가 노는 상태가 된다.
- 이때 웹서버를 클라우드 프론트에게 정보를 제공하는 원천이라는 뜻에서 “Origin”
- 이 Origin의 데이터가 전세계에 있는 클라우드 프론트의 캐시 서버로 분배된다는 뜻에서 클라우드 프론트를 “Distribution” 이라고 부른다.

![Untitled](./assets/images_aws/Untitled%2029.png)

- Web > Create Distribution 설정 입력
    - 웹서버 도메인 등을 입력한다.

![Untitled](./assets/images_aws/Untitled%2030.png)

- 생성된 클라우드 프론트의 도메인 네임으로 이동해보자.
- 클라우드 프론트를 앞 단으로 위치 시켰더니 1초가 걸렸던 로딩 시간이 → **14ms 로 단축**되었다.

![Untitled](./assets/images_aws/Untitled%2031.png)

- 이 때 문제는 웹사이트의 실시간 변경 사항을 반영해주지 못하고 있다는 점이다. 현재 날짜를 가져오는 웹페이지인데 클라우드 프론트로 접속하니 계속 같은 날짜만을 반환해준다. 이는 오리진의 변경 사항을 디스트리뷰션은 모르고 있기 때문에 생기는 문제이다.
- 캐시 설정을 통해 변경해보자.

### 3. 캐시 설정 1

- 클라우드 프론트의 Behavior 설정 >  Edit 클릭

![Untitled](./assets/images_aws/Untitled%2032.png)

- Object Caching 속성 > Use Origin Cache Headers 체크
- 이 속성을 사용해서 `Cache-Control: max-age=60` 이라는 값을 헤더에 포함시키면, 60초 동안 정보가 유효하니 60초 동안에는 다시 요청하지 말라는 의미가 전달되고, 클라우드 프론트는 웹서버에게 데이터를 전달 받고 60초 동안 웹 서버에게 다시 요청하지 않는다.
    
    ![Untitled](./assets/images_aws/Untitled%2033.png)
    
- 웹 브라우저도 마찬가지로 클라우드 프론트로부터 `Cache-Control: max-age=60` 헤더를 가진 웹페이지를 전달 받으므로 웹브라우저는 웹브라우저 대로 클라우드 프론트에 60초 동안 웹페이지를 요청하지 않는다.

![Untitled](./assets/images_aws/Untitled%2034.png)

- 따라서 60초 동안에는 웹서버에게 더 이상 정보를 요청하지 않고 자기 레벨에서 응답을 해주기 때문에 60초 동안 웹서버가 놀 수 있는 상태가 되는 것이다.

### 4. 캐시 설정 2

- 10초에 한번 변경사항을 반영하는 웹사이트를 만들어보자.
- php를 활용해서 `Cache-Control: max-age=10` 속성을 설정한다.

![Untitled](./assets/images_aws/Untitled%2035.png)

- 이제 웹서버 자체로 접속해보자.
- 속성을 적용했지만 `Cache-Control: max-age=0` 으로 헤더가 설정되어있고 아직 접속할 때마다 1초 로딩이 걸린다.
- 이는 새로고침 할 때는 캐시가 적용되지 않기 때문이므로 링크를 클릭해서 이 페이지에 접속하면 캐시가 적용되니, 이 페이지로 이동되는 <a> 태그를 하나 만들고 이 링크를 통해 페이지에 접속하면

![Untitled](./assets/images_aws/Untitled%2036.png)

- 로딩 속도가 6ms로 개선되고 `Cache-Control: max-age=10` 헤더가 적용된 것을 확인할 수 있다.

- 이제 클라우드 프론트로 접속해보자. 우리가 <a> 태그를 만들었는데 변경사항을 반영하지 못하고 있다. 이는 클라우트 프론트의 캐시가 기본적으로 24시간 살아있기 때문이다.
- 24시간을 기다릴 순 없으므로 캐시를 강제로 지우는 방법을 알아보자.

![Untitled](./assets/images_aws/Untitled%2037.png)

### 5. 캐시 설정 3, 캐시 무효화

- 캐시를 강제로 삭제하는 옵션은 CloudFront Distributions > 생성한 클라우드 선택 > Invalidations 탭에서 설정할 수 있다.
    
    ![Untitled](./assets/images_aws/Untitled%2038.png)
    
- Create Invalidation 버튼을 클릭하고, 캐시 무효화를 지정할 경로를 작성한다. (유료 서비스)
    - 우리의 경우 /index.php 를 작성한다.

![Untitled](./assets/images_aws/Untitled%2039.png)

- Invalidation이 모두 적용되고나서 클라우드 프론트로 접속하면 변경 사항이 반영된 모습을 볼 수 있다.
    
    ![Untitled](./assets/images_aws/Untitled%2040.png)
    

# AWS RDS란?



`AWS RDS`는 *Amazon Relational Database Service*의 약자로, 컴퓨터에 데이터 베이스를 설치해주고 대신 운영해주는 서비스이다. RDS 서비스는 비교적 비싸다. 그럼에도 많은 개발자들이 선택하는 데는 이점이 있기 때문이다.

`AWS`에서는 `RDS`를 *Managed* 라고 칭한다. 즉 대신 관리해준다는 이야기다.

데이터베이스를 관리하는 것은 매우 어렵고 위험한 일이며, 데이터 유실, 유출 사고는 어떤 사고보다 치명적이다. 그렇기 때문에 정보 비즈니스에서는 데이터베이스를 빠르고 안전하게 지키기 위해 갖은 노력과 많은 비용을 투자하고 있다. RDS는 이러한 일을 전문 인력에게 위임하는 만큼 RDS 비용이 비싸다.

## RDS 실습

### 1. 데이터 베이스 생성

- AWS > RDS 서비스 검색 > 왼쪽 탭 ‘데이터베이스’ 선택
    
    ![Untitled](./assets/images_aws/Untitled%2041.png)
    
- 데이터베이스 생성 버튼 클릭
    
    ![Untitled](./assets/images_aws/Untitled%2042.png)
    
    - 위 사진과 같이 RDS는 다양한 관계형 데이터베이스들을 제공하고 있다.
- MySQL 선택 > 무료로 진행하기 위해서는 프리티어로 진행 체크
    
    ![Untitled](./assets/images_aws/Untitled%2043.png)
    
- 선택할 수 있는 속성 종류
    - 원하는 DB 버전
    - 인스턴스 클래스
    - 다중 AZ: 가용성 관련, AZ (availability zone), 다른 지역 복제본 생성 여부
    - 스토리지 유형: 데이터 저장 디스크, 범용(SSD) / 프로비저닝 된 IOPS → 비쌈, 빠름
        - 스토리지가 클 수록 속도가 빨라짐
        - 프로비저닝 IOPS는 속도, 용량을 따로 지정할 수 있음 IO → 입출력
- 설정 속성에서 다음 항목 입력
    - DB 인스턴스 식별자
    - 마스터 사용자 이름
    - 마스터 암호

![Untitled](./assets/images_aws/Untitled%2044.png)

- 연결 속성에서 네트워크 및 보안 설정 (VPC)
    - VPC : 기본으로 설정
    - 퍼블릭 액세스 : 예 → 외부에서 접속, 아니오 → VPC 내부에서만 접속
    - VPC 보안 그룹 : 새로운 보안 그룹 만들기
- 추가 구성 > 데이터 베이스 옵션 설정
    - 데이터 베이스 초기 이름 설정
    - 암호화
    - 백업: 자동 백업 생성 보존 기간
- 확장 모니터링: 상태 로그
- 로그 내보내기 지정 가능
- 유지 관리
    - 마이너 버전 업그레이드 → 데이터 베이스 버전 업그레이드
- 삭제 방지
    - 삭제할 때 한 번 방지됨

### VPC란?

![Untitled](./assets/images_aws/Untitled%2045.png)

- AWS 안에서 외부로부터 독립된 안전한 네트워크를 구성해주는 서비스
- VPC를 생성하고 DB 인스턴스를 만들게 되면 외부에서 직접적으로 DB에 접근하는 것을 막을 수 있음
- 같은 VPC안에 AWS를 이용해서 EC2를 생성해서 거기서 데이터 베이스에 접속하게 되면 훨씬 더 안전해질 것
- 위 그림에서 VPC 그룹은 네모 박스 하나라고 생각하면 됨, VPC 안에서도 지정한 머신만 RDS에 접속할 수 있도록 지정 가능

### 2. 퍼블릭 방식으로 접속

- 퍼블릭 접속 설정을 ‘네’로 변경해야 함
- 데이터베이스 > 우상단 ‘수정’ 버튼 클릭 > 퍼블릭 액세스 접속 설정 “예”로 변경
- 그리고 수정 예약을 즉시 적용으로 체크

![Untitled](./assets/images_aws/Untitled%2046.png)

- 엔트 포인트 복사
    
    ![Untitled](./assets/images_aws/Untitled%2047.png)
    
- mysql monitor를 사용할 것, cmd에서 복사한 엔드포인트와 함께 로그인 정보 넘기기
    
    ![Untitled](./assets/images_aws/Untitled%2048.png)
    
- 그런데 접속이 안됨, 이유는 다음과 같음
    
    ![Untitled](./assets/images_aws/Untitled%2049.png)
    
    - AWS에서 방화벽 기능으로 Security group을 제공함
    - MySQL client도 아무나 들어오지 못하게 특정한 IP에서만 접속 가능하도록 지정할 수 있음, 이때 Security group 안에 있는 다양한 서버 중에 RDS로 접속하게 하기 위해 포트 지정해줘야 함
- 데이터 베이스 접속 > 속성 중에 보안 그룹 주소 클릭 > 보안 그룹 체크하면 아래와 같은 속성 보임
    
    ![Untitled](./assets/images_aws/Untitled%2050.png)
    
    - 인바운드: 밖에서 접속
    - 아웃바운드: 응답해주는 것
- 즉 인바운드 설정해주면 됨
    
    ![Untitled](./assets/images_aws/Untitled%2051.png)
    
- 설정 이후 다시 cmd 접속해보면 접속에 성공
    
    ![Untitled](./assets/images_aws/Untitled%2052.png)
    

### 3. 비공개 상태로 접속

- 공개 상태에서 접속하는 것은 위험하다. VPC를 만들어서 그 안에 머신에서 RDS에 접속하도록 설정하는 것이 훨씬 안전하다.
    - 우선 퍼블릭 액세스 끄기
    - 방금 설정한 보안 그룹도 삭제하기
- EC2 인스턴스 생성하기
    - 우분투, t2.micro, vpc를 기본값, 퍼블릭 IP 자동 할당 활성화, 보안 그룹 구성 22번 포트는 SSH라고 해서 CMD에서 접속하려면 22번 포트 열려 있어야 함
        
        ![Untitled](./assets/images_aws/Untitled%2053.png)
        
- SSH로 접속하기
    - CMD에서 다음 명령어 입력하면 ubuntu 서버로 접속 가능
        
        ![Untitled](./assets/images_aws/Untitled%2054.png)
        
    - mysql 입력해보면 설치해야한다고 함
        
        ![Untitled](./assets/images_aws/Untitled%2055.png)
        
    - sudo apt update;
    - sudo apt install mysql-client
    - 데이터베이스 엔드포인트 복사해서 다시 아래 명령어 입력
        
        ![Untitled](./assets/images_aws/Untitled%2056.png)
        
    - 이때 접속이 안되는데 RDS에서 보안 그룹, 인바운드 등록해야함
    - EC2 인스턴스의 IP 주소를 RDS의 Security group에 등록하면됨 혹은 더 좋은 방법으로 EC2의 security group에 등록해도 됨
    - EC2 보안 그룹 ID 카피해오기
        
        ![Untitled](./assets/images_aws/Untitled%2057.png)
        
    - RDS 보안 그룹 > 인바운드  > 편집 > EC2 보안 그룹 ID 복사한 것 붙여넣고 저장
        
        ![Untitled](./assets/images_aws/Untitled%2058.png)
        
- 이제 다시 SSH로 RDS에 접속하려고 하면 접속에 성공하는 것을 확인할 수 있음
    
    ![Untitled](./assets/images_aws/Untitled%2059.png)
    

# Reference

[AWS란? - AWS를 이용한 클라우드 컴퓨팅 - Amazon Web Services](https://aws.amazon.com/ko/what-is-aws/)

[AWS : AWS란?](https://brunch.co.kr/@e9c7009de84443b/102)

[클라우드 컴퓨팅, IaaS, PaaS, SaaS이란?](https://wnsgml972.github.io/network/2018/08/14/network_cloud-computing/)

[[지금 무료] 클라우드 서비스 AWS | Egoing Lee - 인프런](https://www.inflearn.com/course/aws-2/dashboard)

[일반인을 위한 클라우드 용어 해설 IaaS, PaaS, SaaS 차이와 의미](https://skkang520.tistory.com/entry/일반인을-위한-클라우드-용어-해설-IaaS-PaaS-SaaS-차이와-의미)

[클라우드 컴퓨팅 서비스 유형!  IaaS, PaaS, SaaS 가 뭘까요? : 동국시스템즈 포탈 디케이앤유](https://www.dknyou.com/blog/?idx=14931168&bmode=view)