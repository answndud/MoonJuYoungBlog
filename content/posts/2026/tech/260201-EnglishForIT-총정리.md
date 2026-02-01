---
title: “English for IT 총정리”
date: 2026-02-01
draft: false
tags: ["tech", "english”]
categories: ["tech"]
---

# English for IT

## 00. 개요

### 시작하며: 당신이 이 글을 읽어야 하는 이유

### 목차
- 1편: 당신이 당신의 문제를 스스로 만든다
- 2편: 번역기의 배신
- 3편: 영어가 아니라 기술 영어다
- 4편: 단어장이 아니라 문장이다
- 5편: 마스터플랜 - 실전에서 살아남기
- 6편: 녹슬지 않는 기술 영어 만들기

### 시나리오: 나는 영어가 무서워
Spring Security 설정하다가 막혀서 구글링 시작. “Spring Security JWT 설정” 검색하니 한국어 블로그 10개가 나왔습니다. 첫 번째 블로그 따라했더니 에러. 두 번째도 에러. 세 번째는 deprecated 경고…

3시간 삽질 끝에 Spring 공식문서 열었더니 3분만에 해결됐습니다.

“아… 진작 공식문서 볼걸.”

이 후회, 익숙하신가요?

### 우리가 반복하는 실수들
- 월요일: "이 에러 뭔지 모르겠네" → 한국어 블로그 검색 → 2시간 삽질
- 화요일: "새 버전 뭐가 바뀌었지?" → 번역기 돌리기 → 오역으로 혼란
- 수요일: "이 기술 어떻게 쓰지?" → ChatGPT에 물어보기 → 구식 답변
- 목요일: "버그 리포트 해야하는데" → 영어 무서워서 포기
- 금요일: "공식문서 봐야하는데..." → 번역된 블로그 찾기 → 또 삽질

매주 이런 패턴을 반복하면서도 우리는 변하지 않습니다. 왜일까요?

### 영어가 무서워서? 아니다.
진짜 문제는 영어가 아닙니다. 잘못된 믿음이 문제입니다:

#### 착각 1: “영어 잘해야 개발 잘한다”
아닙니다. 기술 문서는 중학교 영어 수준입니다. if, return, throw 같은 단어만 알면 됩니다.

#### 착각 2: “번역기가 다 해결해준다”
번역기는 Semaphore를 신호기로 번역합니다. Promise를 약속으로 번역합니다. 이게 도움이 되나요?

#### 착각 3: “한국어 자료로 충분하다”
GitHub 스타 10k+ 프로젝트와 최신 기술, 논문, 공식문서는 영어로 공유되는것이 대부분입니다. 이 기술들을 전부 놓치고 한국어 자료만 볼 순 없잖아요!

### 이 시리즈를 쓰게 된 이유
개발을 공부하거나, 심지어 현업에 계신 분들마저도 이런 말들을 정말 많이 합니다.

영어 그거 몰라도 개발 잘만 하던데요? 영어공부 정말 죽어도 하기 싫고 필요도 못 느껴요.

글쎄요, 저는 생각이 조금 다릅니다. 영어를 배우지 않고 IT를 공부하는것은 접근 가능한 정보를 스스로 제한하며 공부하는것과 다름이 없거든요.

기술 문서는 문학이 아닙니다. 시를 읽는 게 아니에요. 그냥 설명서입니다. 패턴이 있고, 반복되는 구조가 있습니다.

### 이 시리즈의 목표
거창한 목표 없습니다.

- 원어민처럼 영어 잘하기? ❌
- TOEIC 900점 만들기? ❌
- 영어 회화 마스터? ❌

딱 하나만 목표입니다.

- 기술 문서 번역기 없이 읽기 ✅

이 문서는 영어 이론이 아닌 영어 학습법에 대해 다루겠습니다. 대부분의 경우 학습법만 알려주면 알아서 잘 하거든요.

### 누구를 위한 글인가
이런 분들을 위해 씁니다:

- 매번 한국어 블로그 찾다가 삽질하는 개발자
- 공식문서 보면 머리 아픈 개발자
- 영어 때문에 오픈소스 기여 못하는 개발자
- “영어 공부해야지” 3년째 말만 하는 개발자
- 번역기 없으면 불안한 개발자

### 이 시리즈의 구성
- 1편: 당신이 당신의 문제를 스스로 만든다 왜 한국어 블로그와 ChatGPT가 당신을 삽질하게 만드는지
- 2편: 번역기의 배신 Semaphore가 신호기가 되는 순간, 모든 게 망한다
- 3편: 영어가 아니라 기술 영어다 문법책 버리고 패턴만 익혀라
- 4편: 단어장이 아니라 문장이다 Etymology와 문장 구조로 배우는 실전 영어
- 5편: 마스터플랜 - 실전에서 살아남기 매일 15분, 3개월 로드맵
- 6편: 녹슬지 않는 기술 영어 만들기 실력과 흥미를 동시에 유지하는 법

### 약속
이 시리즈를 다 읽고 나면:

- 왜 공식문서를 봐야 하는지 납득하게 됩니다
- 번역기를 끄고 싶어집니다
- 영어가 그렇게 어렵지 않다는 걸 알게 됩니다
- 오늘 당장 시작할 수 있는 구체적인 방법을 얻습니다
- 최종 마스터플랜을 제시합니다
- 영어를 일상으로 끌어들일수 있게 됩니다

다음: 1편 당신이 당신의 문제를 스스로 만든다 ➡


---

## 01. 당신이 당신의 문제를 스스로 만든다

### 1편: 당신이 당신의 문제를 스스로 만든다

#### 왜 이 글을 쓰게 되었나
3년차, 5년차가 되어도 영어 문서 앞에서 주눅드는 개발자들을 많이 봤습니다. 보통 “영어 잘하는 사람들이나 보는 거 아니야?”라고 생각하며 블로그와 유튜브를 뒤적거리다가, 결국 더 큰 문제를 만들어내는 악순환을 반복하죠. 이 시리즈는 그런 분들을 위한 글입니다.

### 블로그 주도 개발: 지옥의 나날들
처음 웹 개발을 배울때, Spring Boot 구버전에서 Spring Security를 설정하고 있었습니다. JWT 인증을 구현해야 했는데, 한국어 블로그들을 참고해서 이렇게 짰습니다. 자세히는 기억 안 났지만 아마 Tistory 블로그를 참조했던 기억이 납니다.

```java
@Configuration
@EnableWebSecurity
public class WebSecurityConfig extends WebSecurityConfigurerAdapter {
    
    @Override
    protected void configure(HttpSecurity http) throws Exception {
        http.authorizeRequests()
            .antMatchers("/api/auth/**").permitAll()
            .anyRequest().authenticated();
    }
}
```

그러고 나서 컴파일을 하고 서버를 돌리려는데 이런 메시지를 보게 됩니다. deprecated? 이게 다 뭐지.

* 'WebSecurityConfigurerAdapter' is deprecated
* 'configure(HttpSecurity)' is deprecated
* 'authorizeRequests()' is deprecated
* 'antMatchers(String...)' is deprecated

검색해보니 더 이상 지원하지 않는 기술이라 안전하지 않은 기술이라 Bean 기반으로 고쳐야 한다는데… 하 모르겠습니다. 블로그나 검색해보기로 했습니다.

### 삽질의 연속

첫 시도: “Spring Security JWT 인증 구현” 구글링

* 상위 10개 블로그 다 읽음
* 전부 구식 방법 (WebSecurityConfigurerAdapter 상속)
* Stack Overflow도 2019년 답변들만…

두번째 시도: “Spring Boot 2.7 Spring Security 설정” 재검색

* 또 구식 방법들
* YouTube 영상도 전부 옛날 방식
* ChatGPT도 구식 코드 제공

여기서 ChatGPT 얘기를 좀 더 해보자면, ChatGPT나 다른 AI 모델들은 학습 데이터의 시점이 정해져 있습니다. 예를 들어 2023년까지의 데이터로 학습했다면, 2024년에 deprecated된 메서드는 모릅니다. 게다가 학습 데이터의 대부분이 이미 구식이 된 블로그 글들이라면? AI도 구식 코드를 “정답”이라고 알려주게 됩니다. 결국 AI에게 물어봐도 블로그 검색과 똑같은 문제에 빠지는 거죠.

### 3분만에 끝난 해결책

포기하고 Spring Security 공식문서를 열었습니다: [https://spring.io/guides/gs/securing-web/](https://spring.io/guides/gs/securing-web/)

```java
@Configuration
@EnableWebSecurity
public class WebSecurityConfig {

    @Bean
    public SecurityFilterChain filterChain(HttpSecurity http) throws Exception {
        http
            .authorizeHttpRequests((authz) -> authz
                .requestMatchers("/api/auth/**").permitAll()
                .anyRequest().authenticated()
            );
        return http.build();
    }
}
```

별 문제 없이 한번에 해결되는걸 확인할 수 있었습니다. 와. 제가 제 문제를 스스로 만들고 있었군요.

### 왜 이런 일이 반복되나?

#### IT 분야는 오늘 배운게 내일 쓰레기가 됨

웹 개발이나 AI 개발 같은 분야는 변화가 정말 빠릅니다. 물론 안정적이고 검증된 기술을 사용하는 대규모 사업체나 레가시 기술이 중요한 분야는 다르겠지만… 아무튼 실시간으로 업데이트가 가능한 분야 특성상 당장 어제까지 멀쩡하게 쓰던 메서드를 사용하면 경고가 뜨거나, 좀 엄격한 라이브러리의 경우 아예 컴파일 자체를 거부해버리기도 합니다.

많은 개발자들이 개발을 할때 문제가 생기면 ChatGPT에게 묻거나 블로그 글을 검색하곤 합니다. 한국어로 적혀있으니까! 근데 거기 적혀있는거 많은 경우에는, 현재 시점에서는 쓸모가 없는 내용입니다. 현재 시점에서는 업데이트가 되었을 확률이 높기 때문에. 구식 코드를 그대로 사용하면 나중에 문제가 될 수 있습니다. 당장은 작동해도 나중에 큰 문제를 일으킬 수 있어요. 마치 자전거 바퀴에 막대기를 끼우고 넘어지는 것처럼, 의도치 않게 스스로 문제를 만드는 셈입니다.

### 개발자들의 패턴

* 문제 발생
* “한국어로 된 게 없나?” 검색
* 구식/잘못된 정보로 삽질
* 결국 공식문서 참조
* “아, 진작 이거 볼걸…”

### 나만의 경험이 아니다

팀장: “React 18 Suspense 어떻게 쓰지?”

* 한국어 블로그: React 16 방식 안내
* 2시간 삽질 후 React 공식문서 확인
* 5분만에 해결

후배: “Docker multi-stage build 에러”

* Stack Overflow 2020년 답변으로 1일 삽질
* Docker 공식문서 Dockerfile best practices
* 10분만에 해결

동료: “AWS Lambda 콜드 스타트 최적화”

* 개인 블로그 3시간 읽기
* AWS 공식문서 Performance tuning
* 15분만에 핵심 파악

### 최신 정보는 모두 영어로 적혀있음

#### IT 생태계의 진실

* GitHub 스타 10k+ 프로젝트: 많은 경우에 영어로 작성되어있음
* 최신 기술 정보, 논문: 주로 영어로 먼저 공개
* 기술 정보 follow-up을 위한 최대 커뮤니티인 Hacker News: 모두 영어!
* 개인 해커로 활동하며 버그 바운티 활동: 정책이 영어로 적혀있고, PoC도 영어로 작성해야 함
* 공식 문서: 100% 영어 (한국어 번역 있어도 구버전)

### 영어를 공부하는 것이 아닌 기술 영어를 공부하세요

아무리 생각해도 영어를 공부하기 너무 싫을 수 있습니다. 학교에서 영어공부를 했던 경험이 부정적일 수 있고, 언어를 새로 배운다는 것 자체가 방대한 작업으로 느껴질 수 있기 때문입니다.

하지만 생각해보세요. 예를 들면 일본 애니메이션을 본 경험이 있다면, 일본어를 모르기 때문에 일본 애니메이션을 보는 것이 두려웠나요? 그냥 보는것이 재밌으니까 보죠. 그러면서 단어 하나씩 귀에 들리는겁니다. 마나부(배우다), 쿠우(먹다), 아소부(놀다)… 언어를 배우는 작업 자체가 처음부터 완벽하게 하는 것이 아닌 점진적으로 진행되는 일입니다.

우리가 어학시험 만점을 받으려는 것도 아니고 외국인과 자유자재로 대화하려는 것도 아닙니다. 그냥 기술 문서를 읽고 싶은 것뿐입니다.

기술 문서는 일반 영어와 다릅니다. 사용하는 단어도 제한적이고(대략 8천 개 정도 어쩌면 그보다 작음), 문장 구조도 비교적 단순하고 항상 보는 단어만 봅니다. 생각보다 달성 가능한 목표일 수 있습니다.

다른 사람들이 공식 문서 보고 한번에 문제 해결할 때, 우리도 블로그 뒤적거려가며 고생하지 않고 그렇게 할 수 있다면 좋지 않을까요?

---

## 2편: 번역기의 배신

### 공식문서를 번역기로 읽으면 되지 않나?

1편에서 공식문서의 중요성을 강조했더니 이런 질문이 들어올 수 있습니다.

“요즘 번역기 좋아졌는데? ChatGPT도 있고, DeepL도 있고, 구글 번역도 있고… 굳이 영어 공부할 필요 있나? 공식문서도 번역기로 읽으면 되잖아?”

저도 그렇게 생각했습니다. 2025년이면 AI가 완벽하게 번역해줄 줄 알았죠. GPT-5도 있고, Claude도 있고, 번역 특화 AI들도 많은데 뭐가 문제겠어요? 하지만 이런 시나리오를 생각해봅시다. 생각이 좀 달라지실거에요.

### 시나리오 1: 프로덕션 배포 직전의 대참사

한 개발자가 Redis 문서를 번역기로 읽고 있었는데, 이런 문장이 있었습니다(EXPIRE 명령어 설명):

> "Set a timeout on key. After the timeout has expired, the key will automatically be deleted."

번역기 결과:

> "키에 시간 초과를 설정합니다. 시간 초과가 만료된 후, 키는 자동으로 삭제됩니다."

별 문제 없어 보이죠? 저도 그렇게 생각했습니다. 그런데 동료가 제 코드를 리뷰하다가 물어봅니다.

“왜 expire를 1로 설정했어요?”

“문서에 시간 초과를 설정하라고 해서… 1초면 충분할 것 같아서요.”

“…이거 TTL(Time To Live)이에요. 1초 후에 데이터 사라져요.”

“네? 아 그게… 시간 초과가…”

말문이 막혔습니다. “timeout”을 “시간 초과”로 번역하니까 “연결이 끊기는 시간”으로 오해했던 겁니다. 실제로는 “유효 기간”이었는데. 만약 이대로 배포했다면 모든 캐시 데이터가 1초마다 사라지는 대참사가 일어날 뻔했습니다.

### 시나리오 2: 문맥을 정확하게 파악하지 못하는 기계번역

Semaphore는 운영체제/동시성 프로그래밍에서 공유 자원에 동시에 접근할 수 있는 작업(스레드/프로세스)의 ‘허용 가능한 개수’를 제어하는 동기화 기법입니다. 그냥 음차해서 “세마포어”라고 쓰는 것이 표준적이며, 직역해서 신호기라고 하면 의미가 흐려집니다. 특히 GitHub README 같은 곳을 기계번역한 초벌본에서 자주 보이는 실수입니다.

공식 문서(일반적인 정의)에서 흔히 나오는 문장 예:

> A counting semaphore is a type of lock that allows you to limit the number of processes
> that can concurrently access a resource to some fixed number.

이걸 제대로 해석하면: “카운팅 세마포어는 어떤 자원에 동시에 접근할 수 있는 프로세스(혹은 스레드)의 수를 고정된 상한으로 제한하는 락(동기화 수단)의 한 종류다.”

번역기를 그대로 쓰면 종종 신호기 기반 잠금 같이 어색한 표현이 나오고, 개념을 처음 접하는 사람은 ‘신호를 주고받나?’ 같은 잘못된 심상을 가지기 쉽습니다.

예시 - 어떤 오픈소스 프로젝트의 README:

원문:

> "This library uses semaphores to handle concurrent requests.
> The semaphore limits the number of parallel operations to prevent resource exhaustion."

번역기 결과:

> "이 라이브러리는 동시 요청을 처리하기 위해 신호기를 사용합니다.
> 신호기는 자원 고갈을 방지하기 위해 병렬 작업 수를 제한합니다."

이걸 읽고 이해할 수 있나요? 신호기가 대체 뭘 하는 건지…

실제로 일어난 대화:

나: "이 부분 신호기로 처리하면 될 것 같은데요"
팀장: "신호기요? 무슨 신호?"
나: "아... README에서 본 건데... semaphore..."
팀장: "아 세마포어. 번역기로 문서 읽으셨군요."

순간 공기가 얼어붙었습니다.

### 기술 용어 번역의 근본적 한계

#### 1. 도메인 특화 용어

개발에서 쓰는 단어들은 일반적인 뜻과 완전히 다른 경우가 많습니다:

| 영어          | 일반 번역  | 개발에서 의미         | 문제점         |
| ----------- | ------ | --------------- | ----------- |
| thread      | 실      | 스레드 (실행 단위)     | “실을 생성한다”?  |
| memory leak | 기억 누출  | 메모리 누수          | “기억이 샌다”?   |
| cache       | 은닉처    | 캐시 (임시 저장소)     | “은닉처를 비운다”? |
| cookie      | 쿠키(과자) | 쿠키 (웹 데이터)      | “과자를 저장한다”? |
| daemon      | 악마     | 데몬 (백그라운드 프로세스) | “악마를 실행한다”? |

#### 2. 새로운 용어들

기술이 발전하면서 새로 생긴 용어들은 번역 데이터베이스에 없습니다:

* containerization → 번역기: “용기화” / 실제: “컨테이너화”
* orchestration → 번역기: “오케스트라 연주” / 실제: “오케스트레이션”
* serverless → 번역기: “서버 없는” / 실제: “서버리스”
* edge computing → 번역기: “가장자리 컴퓨팅” / 실제: “엣지 컴퓨팅”

#### 3. 문맥 의존적 번역

같은 단어여도 상황에 따라 완전히 다릅니다:

```text
// 'build'의 경우
"build a Docker image" → 도커 이미지를 빌드한다 (O) / 건설한다 (X)
"build a house" → 집을 짓는다 (O) / 빌드한다 (X)

// 'run'의 경우  
"run the application" → 애플리케이션을 실행한다 (O) / 달린다 (X)
"run a marathon" → 마라톤을 뛴다 (O) / 실행한다 (X)
```

2025년 현재 GPT-5, Claude 4, DeepL 같은 최신 AI 번역기도 이런 미묘한 맥락 차이를 완벽하게 구별하지 못합니다.

### 실제 개발할 때 겪는 문제들

#### 검색 결과가 엉망

번역된 용어로 검색하면:

* “신호기 프로그래밍” 검색 → 교통 신호등 제어 시스템 나옴
* “약속 체이닝” 검색 → 결혼 상담소 광고 나옴
* “semaphore programming” 검색 → 제대로 된 자료 나옴
* “promise chaining” 검색 → JavaScript 튜토리얼 나옴

#### Stack Overflow 검색 지옥

실제 경험:

* 한국어로 번역해서 검색: 결과 0개
* 영어로 검색: 정확히 같은 문제 해결한 답변 5개

#### Promise가 “약속”이 되면서 생기는 문제

JavaScript 문서에서 메서드 설명이 이렇게 되어 있다면 어떨까요?:

```text
// 원문
"This method returns a Promise that resolves when the operation completes"

// 번역
"이 메서드는 작업이 완료될 때 해결되는 약속을 반환합니다"
```

이걸 읽고 이해할 수 있나요? 실제 코드와 비교해보면:

```js
// "약속이 해결되면 then을 실행한다"고 이해하면?
fetch('/api/data')
  .then(response => response.json())  // 약속이... 뭐?
  .then(data => console.log(data))    // 그 다음 약속이...?
  .catch(error => console.error(error)); // 약속을 잡는다?

// "Promise가 resolve되면 then을 실행한다"고 이해하면?
fetch('/api/data')
  .then(response => response.json())  // Promise가 성공하면 실행
  .then(data => console.log(data))    // 체이닝된 Promise 처리
  .catch(error => console.error(error)); // Promise rejection 처리
```

어떤 게 더 이해하기 쉬운가요?

### 번역기의 또 다른 함정들

#### 1. 뉘앙스 완전 손실

원문: "This feature is experimental. Use with caution."
번역: "이 기능은 실험적입니다. 주의해서 사용하세요."

실험적이라는 말은 실제로는 서비스 제공자(Provider)가 동작 오류에 대해 책임을 지지 않는다는 의미로 사용하는 경우가 많기 때문에, 직역하면 이상한 의미가 됩니다.

#### 2. 경고 메시지 오독

원문: "DEPRECATED: This will be removed in v3.0"
번역: "사용되지 않음: 이것은 v3.0에서 제거될 것입니다"

Deprecation은 단순히 사용하지 않음을 의미하는 것이 아닌 업데이트 지원 중단으로 권장되지 않는 메서드를 의미합니다.

#### 3. 코드 주석까지 번역되는 재앙

```py
# 원본 코드
# Initialize the connection pool
pool = ConnectionPool()

# 번역기 거친 후
# 연결 수영장을 초기화합니다
pool = ConnectionPool()  # pool이 수영장...?
```

### 결론: 번역기는 보조 도구일 뿐

번역기는 100% 이해했을 때 검증 용도로만 써야 합니다.

잘못된 사용법:

1. 영어 문서 열기
2. 전체 선택 → 번역기 돌리기
3. 번역 결과 맹신하기
4. 이상한 코드 작성
5. 프로덕션 터뜨리기 직전
6. 동료가 구해줌

올바른 사용법:

1. 영어 문서 직접 읽기
2. 모르는 단어만 사전 찾기
3. 이해 안 되는 문장만 번역기 참고
4. 여러 번역 결과 비교
5. 원문과 대조하여 검증
6. 확실히 이해한 후 코드 작성

### 그럼 어떻게 해야 하나?

답: 영어 배우기를 피하지 말자

“번역기 있는데 왜 배워?”가 아니라 “번역기 때문에 더 배워야 한다”

왜냐하면:

* 번역이 맞는지 틀린지 판단하려면 영어를 알아야 함
* 검색할 때 영어 키워드를 써야 제대로 된 자료 나옴
* 동료들과 소통할 때 원래 용어를 알아야 함
* GitHub, Stack Overflow에서 활동하려면 영어 필수
* 새로운 기술 정보는 100% 영어로 먼저 나옴

번역기가 발전해도 개발자가 영어를 배워야 하는 이유는 변하지 않습니다. 오히려 AI 시대가 되면서 더 많은 영어 자료를 더 빠르게 소화해야 하는 상황이 되었죠.

---

## 3편: 영어가 아니라 기술 영어다

### 왜 영어 공부가 실패하는가

1편과 2편을 읽고 “그래, 영어 배워야지!”라고 결심했다가도 막상 시작하려니 막막하실 겁니다.

“토익 책 다시 꺼내야 하나?” “문법책부터 봐야 하나?” “CNN 뉴스 들어야 하나?” “영어 회화 학원 등록해야 하나?”

다 필요 없습니다.

왜냐하면 우리가 배워야 하는 건 ‘영어’가 아니라 ‘기술 영어’니까요.

### 일반 영어 vs 기술 영어: 완전히 다른 세계

#### 일반 영어의 세계

* 필요 어휘: 일상적, 문학적, 학술적 언어 수만 개…
* 문장 구조: 복잡하고 다양함
* 관용구, 속어, 은유 표현 많음
* 문화적 맥락 이해 필요
* 듣기, 말하기, 읽기, 쓰기 모두 필요

#### 기술 영어의 세계

* 필요 어휘: 핵심 단어는 몇천 개 수준
* 문장 구조: 단순하고 반복적
* 관용구 거의 없음, 직설적 표현
* 문화적 맥락 불필요
* 읽기만 하면 됨 (가끔 쓰기)

### 기술 문서에서 실제로 자주 보는 단어들

기술 문서를 읽다 보면 항상 같은 단어들이 반복됩니다:

동작 관련:

* return, call, execute, run, create, initialize, handle, throw, catch

구조 관련:

* function, method, object, array, class, property, value, element

상태 관련:

* true, false, null, undefined, empty, valid, invalid

흐름 관련:

* if, when, then, else, while, for, before, after

이런 단어들만 알아도 문서 읽기가 훨씬 수월해집니다. 일반 영어에서 필요한 2만 개 이상의 어휘와 달리, 기술 문서는 정말 제한적인 어휘를 반복 사용합니다.

### 기술 문서의 문장 패턴

기술 문서는 정말 단순한 패턴을 반복합니다:

패턴 1: X returns Y

* This method returns a Promise
* The function returns an array
* fetch() returns a Response object

패턴 2: X is used to Y

* useState is used to manage state
* This hook is used to fetch data
* The flag is used to enable debugging

패턴 3: If X, then Y

* If the condition is true, the block executes
* If an error occurs, the function throws
* If no match is found, it returns null

이런 패턴들이 계속 반복되는 걸 볼 수 있습니다. 패턴 몇십 개만 익히면 대부분의 문서를 이해할 수 있게 됩니다.

### 마인드셋 전환: 프로그래밍 언어 배우듯이

#### 잘못된 접근

```text
# 영어를 "언어"로 접근
1. 문법 공부 6개월
2. 단어장 외우기 6개월  
3. 리스닝 연습 6개월
4. 회화 연습 6개월
5. 그래도 문서 못 읽음
```

#### 올바른 접근

```text
# 영어를 "도구"로 접근
1. 자주 쓰는 패턴 20개 익히기 (1주)
2. 핵심 단어 500개 익히기 (2주)
3. 실제 문서 읽으며 확장 (계속)
```

프로그래밍 언어 배울 때를 생각해보세요:

* C++ 배울 때 모든 STL을 외우고 시작했나요?
* Python 배울 때 모든 내장 함수를 암기했나요?
* JavaScript 배울 때 ECMAScript 명세서부터 읽었나요?

아니죠. 그냥 if, for, function 같은 기본만 배우고 바로 코딩 시작했잖아요.

### 시작하는 구체적인 방법

#### Step 1: 패턴 인식 훈련 (1주차)

매일 공식 문서 1페이지씩 읽으면서 반복되는 패턴 찾기:

* 월: React 공식문서 - Hooks 페이지
* 화: Node.js 공식문서 - fs module
* 수: MDN - Array methods
* 목: Python 공식문서 - Built-in Functions
* 금: Docker 공식문서 - Getting Started

읽으면서 모르는 단어는 무시하고 구조만 파악합니다. 잘 모르겠으면 ChatGPT한테라도 부탁해보세요. 이 문서에서 자주 사용되는 패턴은 무엇일까? 라고.

#### Step 2: 핵심 단어만 정복 (2-3주차)

모든 단어를 알 필요 없습니다. 자주 나오는 단어들부터 익히세요:

동사 위주로:

* return, call, execute, run, throw, catch, handle…

명사 위주로:

* function, method, object, array, string, error…

형용사 위주로:

* synchronous, asynchronous, deprecated, optional…

접속사/전치사:

* if, when, while, after, before, with, without…

#### Step 3: 실전 투입 (4주차부터)

이제 번역기 끄고 직접 읽습니다:

* 모르는 단어 나와도 일단 넘어가기
* 문맥으로 의미 추측하기
* 정 모르겠으면 그 단어만 검색
* 절대 전체 문장 번역하지 않기

### 학습 가속화 꿀팁

#### 1. 에러 메시지로 시작하기

에러 메시지는 가장 단순한 영어입니다:

* Cannot read property 'x' of undefined
* Expected string but received number
* Missing required parameter 'id'

이런 문장부터 읽기 시작하세요.

#### 2. 코드 주석 읽기

```js
// Initialize the counter
let counter = 0;

// Check if user is authenticated
if (user.isAuthenticated) {
    // Grant access to protected route
    next();
}
```

주석은 핵심만 간단히 적혀있어서 읽기 쉽습니다.

#### 3. Commit 메시지 읽기

* fix: resolve memory leak in connection pool
* feat: add retry logic for failed requests
* docs: update README with installation steps

짧고 명확한 문장들이라 부담이 없습니다.

### 실패하지 않는 비법: 작게 시작하기

첫 주 목표:

* 하루에 에러 메시지 5개 읽기
* 시간: 5분

둘째 주 목표:

* 하루에 공식 문서 1단락 읽기
* 시간: 10분

셋째 주 목표:

* 하루에 공식 문서 1페이지 읽기
* 시간: 15분

이렇게 하면 3개월 후:

* 기술 문서 술술 읽음
* Stack Overflow 답변 이해함
* GitHub Issues 작성 가능

### 마인드셋 정리

❌ “영어 잘해야 개발 잘한다” ✅ “기술 용어만 알면 문서 읽는다”

❌ “문법부터 완벽하게” ✅ “패턴 파악하고 바로 실전”

❌ “모든 단어 암기” ✅ “핵심 단어 500개만”

❌ “영어 못하면 창피해” ✅ “틀려도 되니까 일단 읽자”

---

## 4편: 단어장이 아니라 문장이다

### 내가 단어장을 한 번도 안 쓴 이유
저는 태어나서 단 한 번도 영어 단어장으로 공부한 적이 없습니다. 대신 롱맨(Longman) 영영사전과 실제 텍스트(논문, 블로그, 시험 문제)로만 공부했습니다. 단어장을 사 본 적은 있는데 하루 이상 쳐다보지 않았습니다. 지루하니까요. 여러분도 단어장 쳐다보고 있기 싫잖아요?

### Play의 비극: 단어장이 만드는 재앙
이를테면 play를 “놀다”로 해석한 ESL(제 2외국어로서의 영어) 학습자가 다음과 같은 문장을 영작한다고 해봅시다.

음, 나 혼자 노는거 좋아해!

그래서 영작을 할때 이렇게 생각합니다. 논다는 단어는 뭐가 좋을까. play? 그럼 이렇게 쓰면 되겠다.

"Um, I want to play with myself!"

하지만 이렇게 쓰면… 변태로 몰릴 수 있습니다. 영어에서 ‘play with’는 성적인 뉘앙스를 담을 수 있기 때문입니다.

단어장에는 이렇게 써있었을 겁니다:

play: 놀다, 연주하다, 경기하다

기술 문서에서는:

- "play a role" - 역할을 하다
- "play nice with" - 호환되다
- "play around" - 실험해보다 (informal)
- "play it safe" - 안전하게 하다

단어장에 적힌 단어는 죽은 단어입니다. 문맥이 없이 단어만 있으면 무슨 소용일까요? 특히 우리는 기술 분야에서만 영어를 볼 것이라고 생각하면 더더욱 그렇습니다.

### 문장으로 배워야 하는 진짜 이유

#### 1. 컨텍스트가 의미를 결정한다
```text
// "return"의 다양한 의미
return value;        // 값을 반환하다
return early;        // 일찍 종료하다  
return to sender;    // 발신자에게 되돌리다 (이건 프로그래밍 아님)
```

#### 2. 콜로케이션(연어)를 자연스럽게 익힌다

단어장으로는 절대 못 배우는 것들:

* throw an exception (예외를 던지다) ✅

* throw an error (에러를 던지다) ✅

* throw a mistake ❌ (이런 표현 없음)

* make a request (요청을 만들다) ✅

* do a request ❌ (이런 표현 없음)

* perform a request (요청을 수행하다) ✅

#### 3. 문법이 저절로 체득된다

문장을 통째로 읽으면:

"This function returns a promise that resolves when..."

* function은 단수니까 returns
* that 이하는 promise를 설명
* when은 시간 조건

이걸 문법책으로 배우면 3개월, 문장으로 읽으면 3초.

### Etymology(어원)로 단어 뜻 유추하기

어원이 뭘까요? 한국어로 치면 우리는 나 어제 밥 먹었어. 라는 문장을 구사한다면 ‘먹었어’는 ‘먹다’의 변형이 됩니다. 이때 이 원형이 되는 ‘먹다’라는 단어가 어근이 됩니다.

영어도 마찬가지로 이런 어근이 있습니다. shocking(충격적인)이라는 단어는 shock(충격) + -ing(형용사형 분사화 접사)로 구성이 되죠. 영어단어는 이런 어근의 결합으로 많이 구성이 되기 때문에 자주 사용되는 몇몇 어근을 암기해두면 외워야 할 단어수가 많이 줄어듭니다.

co-work, co-efficient, co-porate 등 아하, co-라는 어근은 함께한다는 뜻이니까 뭔가 함께하거나 상호작용이 있는거겠구나. 라고 의미를 부분적으로라도 생각해보고, 문맥 속에서 무슨 뜻인지 짐작이라도 해볼수 있으니, 실제로 당장 암기하지 않은 단어라도 깨우칠 가능성이 있는거죠.

예를 들어 다음과 같은 단어들을 생각해봅시다:

* Synchronous = syn + chron + ous

  * syn: 함께 (synthesis, syndrome)
  * chron: 시간 (chronology, chronic)
  * ous: ~한 성질의 → “함께 시간을 맞춘” = 동기적

* Asynchronous = a + syn + chron + ous

  * a: 부정 (없음) → “시간을 맞추지 않은” = 비동기적

* Initialize = init + ial + ize

  * init: 시작 (initiate)
  * ial: ~의
  * ize: ~하게 만들다 → “시작 상태로 만들다” = 초기화하다

* Deprecated = de + prec + ated

  * de: 아래로, 반대로
  * prec: 가치 (precious, price)
  * ated: ~된 → “가치가 떨어진” = 더 이상 권장하지 않는

그럼 이런 어근 학습을 어떻게 하냐고요? 우선은 요즘은 구글도 단어 검색을 하면 etymology 분석을 기본적으로 해주니 단어마다 etymology 분석을 해봐도 좋고… 자주 사용하는 etymology 자체는 외우면 좋은건 사실입니다.

제가 단어장은 사지 마라고 했지만 어근, 어원 단어장에 대해서는 좀 예외를 두고 싶습니다. 수능용 어근/어원 단어장은 많으니 직접 추천하긴 어렵지만 검색해보면 많이 나올거에요.

### 실전 학습법: 모르는 단어 관리

* 단어장 구매 ❌
* 실제 문장에서 발견한 단어만 ✅

나만의 플래시카드 만들기:

앞면:
"The function throws an exception when the input is invalid"

뒷면:

* throws: (예외를) 발생시키다
* exception: 예외 (정상적이지 않은 상황)
* invalid: 유효하지 않은

왜 문장째로 저장하나?

* 단어가 쓰이는 맥락을 기억
* 문법 구조도 함께 익힘
* 실제 사용 예시를 체득

### 추천 학습 자료 (2025년 기준)

#### 사전

* Longman Dictionary of Contemporary English: 간단한 영어로 설명
* Cambridge Dictionary: 프로그래밍 용어 설명 good
* MDN Glossary: 웹 개발 용어 전문

#### 읽을거리 (난이도 순)

* GitHub README 파일들: 짧고 명확
* 공식 문서의 Getting Started: 초보자 대상이라 쉬움
* Stack Overflow accepted answers: 실용적인 영어
* Tech 블로그 (Medium, Dev.to): 구어체 섞인 기술 영어
* RFC 문서: 고급자용, 정확한 기술 영어

#### 피해야 할 자료

* TOEIC/TOEFL 단어장
* 일반 영어 회화책
* 비즈니스 영어 교재
* 옛날 프로그래밍 책의 번역서

### 문장 패턴 20선 (외우지 말고 익숙해지기)

1. X is used to Y
2. X is designed for Y
3. X returns Y
4. X throws Y when Z
5. If X, then Y
6. X must be Y before Z
7. X can be Y or Z
8. X should not be null
9. This allows X to Y
10. X is responsible for Y
11. X depends on Y
12. X is required for Y
13. Make sure X before Y
14. X happens when Y
15. X prevents Y from Z
16. Either X or Y
17. X is called when Y
18. X is triggered by Y
19. By default, X
20. X is expected to Y

이 패턴들을 단어장처럼 외우는 게 아니라, 문서 읽으면서 “아 또 이 패턴이네” 하고 인식하는 겁니다.

### 실제 적용 예시

React 문서의 한 문장:

"This Hook returns a stateful value and a function to update it."

단어장식 해석: “이 갈고리는 상태가 있는 값과 그것을 업데이트하는 함수를 반환한다” → 갈고리? 상태가 있는 값?

문장 학습식 이해: “이 Hook은 상태값과 그것을 업데이트하는 함수를 반환한다” → Hook은 그냥 Hook, stateful은 상태를 가진

차이가 느껴지시나요?

### 마무리: 영어는 도구다

개발할 때 변수명 지을 때도 우리는 이미 영어를 씁니다:

* getUserById()
* handleClickEvent()
* isValidEmail()

이것도 문장입니다. 우리는 이미 영어 문장을 만들고 있어요.

기술 영어도 똑같습니다. 문장을 읽으세요. 패턴을 익히세요. 단어장은 버리세요.

---

## 5편: 마스터플랜 - 실전에서 살아남기

### 이제 진짜 시작이다

1편부터 4편까지 읽으셨다면 이미 마음가짐은 준비되셨을 겁니다. 공식문서의 중요성도 알고, 번역기의 함정도 알고, 기술 영어가 뭔지도 알고, 문장으로 배워야 한다는 것도 알죠.

그런데 막상 시작하려니 막막하실 겁니다.

“그래서… 오늘 뭐부터 하지?”

이제 구체적인 액션 플랜을 제시합니다. 3개월 안에 기술 문서를 번역기 없이 읽을 수 있는 마스터플랜입니다.

### Phase 1: 워밍업 (1-2주)

#### Day 1-3: 현재 레벨 체크

월: React 공식문서 Introduction 읽기

* 몇 %나 이해했는지 스스로 평가
* 모르는 단어 10개만 메모

화: 같은 문서 다시 읽기

* 어제보다 더 이해되는지 확인
* 반복되는 패턴 찾기

수: 다른 프레임워크 문서 Introduction 읽기

* Vue, Angular, Svelte 중 택 1
* 비슷한 패턴이 보이는지 확인

#### Day 4-7: 기본 패턴 체득

매일 15분씩 투자:

```text
// 이런 주석들을 영어로 바꿔보기
// 사용자 정보를 가져온다
// fetchUserInfo()

// 에러가 발생하면 null을 반환한다
// if (error) return null;

// 비동기로 데이터를 처리한다
// await processDataAsync();
```

답:

```text
// Fetch user information
// Return null if error occurs  
// Process data asynchronously
```

이거 하면서 느낄 겁니다. “어? 생각보다 단순한데?”

### Phase 2: 실전 투입 (3-6주)

#### 매일 루틴 (15분)

* 아침 5분: GitHub Trending 프로젝트 README 1개 읽기
* 점심 5분: Stack Overflow 질문 1개 + 답변 1개 읽기
* 저녁 5분: 관심 라이브러리 changelog 읽기

#### 주간 미션

월요일: Error 메시지 수집

실제 개발하다 만난 에러 메시지 5개를 영어로 정리
"Cannot read property 'x' of undefined"
→ undefined의 x 속성을 읽을 수 없다
→ 왜 이런 에러가 나는지 영어로 설명해보기

수요일: PR 코멘트 연습

오픈소스 프로젝트에서 PR 하나 골라서 코멘트 읽기
"This looks good to me"
"Could you add some tests?"
"Please rebase with main branch"
→ 이런 표현들 노트에 정리

금요일: 나만의 README 작성

```md
# My Project

## Description
This project helps developers to...

## Installation

**npm install my-project**

## Usage

**run docker...**
```

처음엔 3줄도 힘들 겁니다. 괜찮아요. 3개월 후엔 30줄도 쓸 수 있을 거예요.

### Phase 3: 레벨업 (7-12주)

#### 실전 미션 리스트

Level 1: 읽기만

* React 새 기능 문서 읽고 요약하기
* Node.js 보안 업데이트 읽고 이해하기
* Docker 베스트 프랙티스 문서 완독

Level 2: 상호작용

* GitHub Issue에 버그 리포트 작성 (영어로)
* Stack Overflow에 질문 올리기
* 오픈소스 프로젝트에 오타 수정 PR

Level 3: 창작

* 기술 블로그 포스트 1개 영어로 작성
* 내 프로젝트 영문 문서 작성
* Dev.to나 Medium에 글 투고

### ChatGPT/Claude 활용법 (보조 도구로만!)

좋은 활용:

* "이 문장 구조를 분석해줘:
  'This method returns a promise that resolves when...'"
* "이 두 표현의 뉘앙스 차이가 뭐야?
  'should be' vs 'must be'"
* "내가 쓴 이 문장이 자연스러운지 확인해줘:
  'This function is making the array to be sorted'"

나쁜 활용:

* "이 문서 전체 번역해줘"
* "이거 요약해줘"
* "이해 안 되니까 쉽게 설명해줘"

그리고 LLM의 문맥 파악 능력은 제한적이기 때문에, 꼭 답변을 실제로 검색해서 맞는 이야기인지 검증해주세요.

### 마지막 당부: 당신이 좋아하는 영어 텍스트를 읽으세요

영어는 재능이 아니라 노출의 문제입니다. 매일 15분씩 3개월이면 22.5시간. 하루에 3시간씩 일주일 공부하는 것과 같은 시간입니다. 하지만 효과는 훨씬 큽니다.

왜냐하면:

* 매일 하면 잊어버릴 틈이 없음
* 실제 필요한 것만 배움
* 바로 써먹을 수 있음
* 성취감이 즉시 느껴짐

하지만 습관적으로 영어를 읽는 루틴을 만들기가 쉽지 않습니다. 특히 강제력이 없다면요. 그렇기 때문에 자발적으로 영어를 읽을 수 있는 기회를 하나쯤 만들어두시면 크게 도움이 됩니다.

영어로 된 소설이든 신문이든 기술 블로그든 당신이 좋아하는 텍스트를 읽으세요. 그게 가장 영어를 쉽고 빠르게 공부하고, 그리고 영어 공부 자체를 습관화하는 방법입니다.

### 실패해도 괜찮다

3개월 플랜을 시작했다가 며칠 못 하고 그만둬도 괜찮습니다. 다시 시작하면 되니까요.

중요한 건 “영어 못 해서 개발 못 한다”, “영어 안 해도 개발할 수 있다”는 변명을 그만두는겁니다.

오늘 GitHub Trending 페이지 열어보는 것부터 시작해보시겠어요?

“The best time to plant a tree was 20 years ago. The second best time is now.”

나무를 심기 가장 좋은 때는 20년 전이었다. 두 번째로 좋은 때는 바로 지금이다.

영어도 마찬가지입니다. 시작하세요. 지금 당장.

---

## 6편: 녹슬지 않는 기술 영어 만들기

### 3개월의 마법, 그 후의 현실

5편까지 따라오셨다면 이제 공식문서를 읽을 수 있게 되셨을 겁니다. 축하드립니다! 그런데…

언어는 근육과 같습니다. 안 쓰면 금방 퇴화해요.

그럼 앞으로도 영어를 꾸역꾸역 계속 해야 하나요?
1편에서 말했듯이 사람들은 종종 스스로의 문제를 스스로 만듭니다. 꾸역꾸역 하면 당연히 하기 싫죠.

강제력을 띄는 학습은 길게 가지 못합니다. 즐길 수 있어야 오래할수 있어요. 제가 5편에서 좋아하는 텍스트를 읽어라고 했죠?

예를 들면 이런 것들을 해보세요:

* GothamChess같은 재밌는 유튜버의 체스 방송 보기
* Hacker News에서 드라마 같은 스타트업 망한 썰 읽기
* Reddit r/programming에서 개발자들 키배 구경하기
* GitHub issue에서 maintainer와 contributor 싸우는 거 보기
* Stack Overflow에서 Jon Skeet의 전설적인 답변 읽기

“아, 재밌는 걸 듣고, 읽으면 되는구나!”

뭐 평소에 기술 관련 글은 죽어도 읽기 싫다면, 좋아요. 안 읽어도 돼요. 대신 당신이 좋아하는 텍스트를 찾으세요! 애니메이션이든, 소설이든, 영화든… 사실 하나쯤은 있을거에요.

### 개발자를 위한 영어 유지 전략

#### 재미로 시작하기

Before (의무감):
"오늘도 영어 공부해야지... Medium 기술 아티클 읽어야지..."
→ 3일 만에 포기

After (재미):
"와 이 사람 PostgreSQL로 Doom 돌렸대 ㅋㅋㅋ"
"Rust vs Go 또 싸우네, 댓글 구경 가야지"
→ 자연스럽게 매일 읽게 됨

### 내가 실제로 하는 루틴

#### 아침에 일어나서 디스코드 웹훅으로 온 해커뉴스 확인

Hacker News 훑어보기

* 제목만 봐도 재밌는 거 클릭
* "Show HN: I built..." 포스트 구경
* 댓글에서 진짜 인사이트 얻기

#### 점심 먹으면서

GitHub Trending 구경

* Star 폭발한 프로젝트 README 읽기
* "왜 갑자기 뜨지?" 궁금증 해결
* Issue 탭에서 사람들 반응 보기

#### 자기 전 (15분)

Reddit 개발 서브레딧

* r/programminghumor (개발자 밈)
* r/cscareerquestions (연봉 자랑 & 고민)
* r/webdev (최신 트렌드 논쟁)

이게 공부인가요? 아니에요. 그냥 재밌어서 보는 거예요. 근데 이게 쌓이면 영어 실력이 됩니다.

### 영어를 쓸 수밖에 없는 환경 만들기

#### 수동적이지만 필수인 것들

```text
// 이전: 한글 주석
// 사용자 정보를 가져오는 함수

// 이후: 영어 주석 (commit 메시지도)
// Fetch user information from database
// Returns null if user doesn't exist
```

VSCode 설정도 영어로:

* 에러 메시지가 영어로 나옴
* 구글링할 때 복붙하기 편함
* 자연스럽게 영어 표현 익힘

#### 능동적이지만 부담 없는 것들

GitHub에서 놀기:

* Level 1: Star 누르고 Watch하기
* Level 2: Issue에 "Thanks! This helped me" 댓글
* Level 3: README 오타 수정 PR
* Level 4: 버그 리포트 작성
* Level 5: 기능 제안하기

### 실패해도 되는 이유

원어민들도 문법 틀립니다. 여러분들은 한국어 문법을 존중하나요? 띄어쓰기를 철저하게 지켜 글을 작성하나요? 그러지 않죠. 당신의 목적은 영어 시험을 보는게 아니라 소통이니, 좀 틀려도 대개 의미가 통합니다. 누가 문법 틀렸다고 하면 이렇게 말하세요. "난 너희랑 소통하려고 영어 배우는건데 문법까지 배우라고 하냐? 너희가 한국어 배워와!"

결론: 개발자들은 문법 신경 안 씀. 코드가 맞으면 됨.

### 이 모든 걸 가능하게 하는 마인드셋

#### ❌ 하지 말아야 할 생각

* “영어 실력 유지해야지” (의무감)
* “매일 1시간씩 공부해야지” (부담)
* “완벽한 영어 써야지” (압박)

#### ✅ 가져야 할 생각

* “이거 재밌겠는데?” (호기심)
* “남들은 뭐라고 하지?” (관심)
* “나도 한마디 해볼까?” (참여)

### 진짜 마지막 조언

동료가 물어봤습니다: “영어 어떻게 유지해요?”

“유지한다고 생각한 적 없는데… 그냥 재밌는 거 보다 보니까?”

이게 정답입니다. 유지하려고 하지 마세요. 즐기세요.

프로그래밍도 그렇잖아요. “코딩 실력 유지해야지”라고 생각하면서 코딩하나요? 아니죠. 만들고 싶은 게 있어서, 궁금한 게 있어서, 문제를 해결하고 싶어서 코딩하죠.

영어도 똑같습니다.

### 오늘 당장 시작하기

* Hacker News 북마크하기
* Reddit 계정 만들기 (lurker로 시작해도 OK)
* GitHub Trending 페이지 열어보기
* 재밌어 보이는 거 하나 클릭

이게 끝입니다.

“영어 유지”가 아니라 “개발 문화 즐기기”라고 생각하세요.

어차피 우리가 좋아하는 개발 이야기는 다 영어로 먼저 나오니까요.
