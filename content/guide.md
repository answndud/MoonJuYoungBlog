---
title: "블로그 운영 가이드"
date: 2026-01-28
draft: true
description: "Hugo 블로그 운영을 위한 종합 가이드입니다."
---

## 목차

1. [폴더 구조 이해하기](#폴더-구조-이해하기)
2. [새 글 작성하기](#새-글-작성하기)
3. [Front Matter 완벽 가이드](#front-matter-완벽-가이드)
4. [이미지 및 미디어 관리](#이미지-및-미디어-관리)
5. [태그와 카테고리 관리](#태그와-카테고리-관리)
6. [SEO 최적화](#seo-최적화)
7. [배포 프로세스](#배포-프로세스)
8. [로컬 개발 환경](#로컬-개발-환경)
9. [테마 커스터마이징](#테마-커스터마이징)
10. [고급 기능](#고급-기능)
11. [문제 해결](#문제-해결)

---

## 폴더 구조 이해하기

```
github_blog/
├── archetypes/          # 새 글 생성 시 사용되는 템플릿
│   └── default.md
├── content/             # 📝 블로그 콘텐츠 (주로 여기서 작업)
│   ├── posts/           # 블로그 포스트
│   ├── archives.md      # 아카이브 페이지
│   └── search.md        # 검색 페이지
├── static/              # 정적 파일 (이미지, 파일 등)
├── themes/              # Hugo 테마
│   └── PaperMod/
├── public/              # 빌드 결과물 (자동 생성, Git 무시)
├── .github/
│   └── workflows/       # GitHub Actions 워크플로우
├── hugo.toml            # 사이트 설정 파일
└── README.md
```

### 주요 폴더 설명

| 폴더 | 역할 | 수정 빈도 |
|------|------|----------|
| `content/` | 블로그 글, 페이지 저장 | 매우 자주 |
| `static/` | 이미지, 다운로드 파일 | 자주 |
| `hugo.toml` | 사이트 전체 설정 | 가끔 |
| `themes/` | 테마 파일 (수정 비권장) | 거의 없음 |

---

## 새 글 작성하기

### 방법 1: 직접 파일 생성 (권장)

`content/posts/` 폴더에 `.md` 파일을 직접 생성합니다.

```markdown
---
title: "나의 첫 번째 글"
date: 2026-01-28
draft: false
---

본문 내용을 여기에 작성합니다.
```

### 방법 2: Hugo 명령어 사용

```bash
hugo new posts/my-new-post.md
```

이 명령어는 `archetypes/default.md` 템플릿을 기반으로 새 파일을 생성합니다.

### 파일명 규칙

- **소문자 사용**: `my-post.md` ✓ / `My Post.md` ✗
- **공백 대신 하이픈**: `hello-world.md` ✓ / `hello world.md` ✗
- **의미 있는 이름**: URL에 그대로 반영됩니다
  - `content/posts/hello-world.md` → `/posts/hello-world/`

---

## Front Matter 완벽 가이드

Front Matter는 글 상단의 `---`로 감싸진 메타데이터입니다.

### 기본 필드

```yaml
---
title: "글 제목"                    # 필수
date: 2026-01-28                   # 필수, 작성일
draft: false                       # true면 배포에서 제외
---
```

### 확장 필드

```yaml
---
title: "완벽한 Front Matter 예시"
date: 2026-01-28T15:30:00+09:00    # 시간까지 지정 가능
lastmod: 2026-01-29                # 마지막 수정일
draft: false
weight: 1                          # 정렬 순서 (낮을수록 위)

# 분류
tags: ["Hugo", "블로그", "튜토리얼"]
categories: ["개발"]

# SEO 관련
description: "이 글의 요약 설명입니다. 검색 결과와 소셜 공유에 표시됩니다."
keywords: ["Hugo", "블로그 만들기", "GitHub Pages"]

# 표시 옵션
author: "작성자 이름"
showToc: true                      # 목차 표시
TocOpen: false                     # 목차 기본 열림/닫힘
hidemeta: false                    # 메타정보 숨김
comments: true                     # 댓글 활성화 (설정 필요)

# 커버 이미지
cover:
  image: "/images/cover.jpg"       # 커버 이미지 경로
  alt: "이미지 설명"
  caption: "이미지 캡션"
  relative: false
---
```

### Draft (초안) 활용하기

```yaml
draft: true   # 배포 시 제외, 로컬에서만 확인 가능
draft: false  # 배포에 포함
```

- `hugo server -D`: draft 포함하여 로컬 미리보기
- `hugo server`: draft 제외하여 로컬 미리보기

---

## 이미지 및 미디어 관리

### 방법 1: static 폴더 사용 (권장)

```
static/
└── images/
    ├── posts/
    │   └── my-post/
    │       ├── cover.jpg
    │       └── screenshot.png
    └── profile.jpg
```

마크다운에서 사용:

```markdown
![이미지 설명](/images/posts/my-post/screenshot.png)
```

### 방법 2: 페이지 번들 사용

포스트와 이미지를 함께 관리하는 방법:

```
content/posts/
└── my-post/
    ├── index.md          # 글 내용
    ├── cover.jpg
    └── diagram.png
```

마크다운에서 상대 경로로 참조:

```markdown
![다이어그램](diagram.png)
```

### 이미지 최적화 팁

1. **적절한 크기**: 가로 1200px 이하 권장
2. **압축**: [TinyPNG](https://tinypng.com/), [Squoosh](https://squoosh.app/) 사용
3. **WebP 형식**: 용량 대비 품질이 우수
4. **Alt 텍스트**: 항상 의미 있는 설명 작성 (SEO, 접근성)

---

## 태그와 카테고리 관리

### 태그 vs 카테고리

| 구분 | 태그 (Tags) | 카테고리 (Categories) |
|------|------------|---------------------|
| 용도 | 세부 키워드 | 큰 분류 |
| 개수 | 여러 개 가능 | 1-2개 권장 |
| 예시 | Python, Django, REST API | 개발, 일상 |

### 사용 예시

```yaml
---
title: "Django REST API 만들기"
tags: ["Python", "Django", "REST API", "백엔드"]
categories: ["개발"]
---
```

### 일관성 유지하기

태그는 일관된 형식으로 사용하세요:

```yaml
# 좋은 예 - 일관된 형식
tags: ["JavaScript", "React", "TypeScript"]

# 나쁜 예 - 불일관
tags: ["javascript", "REACT", "type-script"]
```

---

## SEO 최적화

### 1. 기본 SEO 설정 (hugo.toml)

```toml
[params]
description = "블로그 전체 설명"
keywords = ["키워드1", "키워드2"]
author = "작성자 이름"

# Open Graph / 소셜 미디어
images = ["/images/og-image.jpg"]
```

### 2. 개별 글 SEO

```yaml
---
title: "검색에 잘 노출되는 제목 작성법"  # 60자 이내 권장
description: "이 글의 핵심을 담은 설명. 검색 결과에 표시됩니다."  # 160자 이내
keywords: ["핵심 키워드", "관련 키워드"]
---
```

### 3. URL 구조 최적화

```yaml
# 기본 URL: /posts/my-long-post-title/
# 커스텀 URL 지정:
slug: "short-url"  # /posts/short-url/
# 또는
url: "/custom/path/"  # /custom/path/
```

### 4. 제목 작성 팁

```markdown
# H1 제목 (페이지당 1개만, title과 동일하게)

## H2 소제목 - 주요 섹션 구분

### H3 하위 제목

#### H4 세부 항목
```

- H1은 글당 1개만 사용 (title이 H1 역할)
- 계층 구조를 지켜서 작성
- 키워드를 자연스럽게 포함

### 5. 내부 링크 활용

```markdown
관련 글: [Hugo 시작하기](/posts/getting-started-hugo/)
```

내부 링크는 SEO에 도움이 되고 독자의 체류 시간을 늘립니다.

### 6. 이미지 SEO

```markdown
![Django REST Framework 아키텍처 다이어그램](/images/drf-architecture.png)
```

- Alt 텍스트에 키워드 포함
- 파일명도 의미 있게: `drf-architecture.png` ✓ / `image1.png` ✗

### 7. robots.txt 및 sitemap

Hugo가 자동으로 생성합니다:
- `https://your-blog.github.io/sitemap.xml`
- `https://your-blog.github.io/robots.txt`

### 8. Google Search Console 등록

1. [Google Search Console](https://search.google.com/search-console) 접속
2. 속성 추가 → URL 접두어 방식 선택
3. HTML 태그 인증 또는 DNS 인증
4. sitemap.xml 제출: `https://your-blog.github.io/sitemap.xml`

### 9. 소셜 미디어 미리보기

글에 커버 이미지를 설정하면 SNS 공유 시 썸네일이 표시됩니다:

```yaml
cover:
  image: "/images/posts/my-post/cover.jpg"
  alt: "포스트 커버 이미지"
```

---

## 배포 프로세스

### 자동 배포 (GitHub Actions)

1. 로컬에서 글 작성/수정
2. Git 커밋 및 푸시:

```bash
git add .
git commit -m "새 포스트: Hugo SEO 가이드"
git push
```

3. GitHub Actions가 자동으로:
   - Hugo 빌드 실행
   - 정적 파일 생성
   - GitHub Pages에 배포

4. 1-2분 후 블로그에 반영

### 배포 상태 확인

- GitHub 저장소 → **Actions** 탭에서 빌드 상태 확인
- 녹색 체크: 성공 ✓
- 빨간 X: 실패 (로그 확인 필요)

### 배포 실패 시

1. Actions 탭에서 실패한 워크플로우 클릭
2. 로그에서 에러 메시지 확인
3. 주로 발생하는 문제:
   - Front Matter 문법 오류
   - 존재하지 않는 이미지 참조
   - hugo.toml 설정 오류

---

## 로컬 개발 환경

### Hugo 서버 실행

```bash
# 기본 실행
hugo server

# draft 포함
hugo server -D

# 특정 포트 지정
hugo server -p 1234

# 모든 IP에서 접근 허용 (모바일 테스트용)
hugo server --bind 0.0.0.0
```

### 빌드만 실행

```bash
hugo
```

`public/` 폴더에 정적 파일이 생성됩니다.

### 유용한 명령어

```bash
# 새 글 생성
hugo new posts/new-post.md

# 버전 확인
hugo version

# 설정 확인
hugo config
```

---

## 테마 커스터마이징

### 색상 변경

`assets/css/extended/` 폴더를 만들고 CSS 파일 추가:

```
assets/
└── css/
    └── extended/
        └── custom.css
```

```css
/* assets/css/extended/custom.css */
:root {
    --primary: #1e90ff;  /* 메인 색상 */
    --secondary: #6c757d;
}
```

### 레이아웃 커스터마이징

테마 파일을 직접 수정하지 말고, `layouts/` 폴더에 동일한 경로로 파일을 만들어 오버라이드:

```
layouts/
└── partials/
    └── footer.html  # themes/PaperMod/layouts/partials/footer.html 오버라이드
```

### 파비콘 설정

`static/` 폴더에 파비콘 파일 추가:

```
static/
├── favicon.ico
├── favicon-16x16.png
├── favicon-32x32.png
├── apple-touch-icon.png
└── safari-pinned-tab.svg
```

[Favicon Generator](https://realfavicongenerator.net/)에서 생성 가능

---

## 고급 기능

### 1. 시리즈 글 작성

```yaml
---
title: "Django 튜토리얼 Part 1"
series: ["Django 완벽 가이드"]
series_order: 1
---
```

### 2. 수학 수식 (KaTeX)

`hugo.toml`에 추가:

```toml
[params.math]
enable = true
```

마크다운에서 사용:

```markdown
인라인: $E = mc^2$

블록:
$$
\sum_{i=1}^{n} x_i = x_1 + x_2 + \cdots + x_n
$$
```

### 3. 코드 하이라이팅

````markdown
```python {linenos=true,hl_lines=[2,4]}
def hello():
    print("Hello")  # 강조
    x = 1
    return x        # 강조
```
````

### 4. 단축코드 (Shortcodes)

YouTube 영상 삽입:

```markdown
{{</* youtube VIDEO_ID */>}}
```

트위터 삽입:

```markdown
{{</* twitter TWEET_ID */>}}
```

### 5. 댓글 시스템 (Giscus)

이 블로그는 **Giscus**를 사용해 GitHub Discussions 기반 댓글 기능을 제공합니다.

#### 설정 방법

**1단계: GitHub 저장소 설정**

1. [저장소 설정](https://github.com/answndud/MoonJuYoungBlog/settings)에서 **Discussions** 활성화
2. [Giscus 앱](https://github.com/apps/giscus) 설치 및 저장소 권한 부여

**2단계: 설정값 확인**

[Giscus 설정 페이지](https://giscus.app/ko)에서:
- 저장소: `answndud/MoonJuYoungBlog` 입력
- 페이지 ↔️ Discussion 연결: `pathname` 선택
- Discussion 카테고리 선택
- 생성된 설정값을 `hugo.toml`에 적용

**3단계: 현재 설정 (hugo.toml)**

```toml
[params]
comments = true  # 전역 댓글 활성화

[params.giscus]
repo = "answndud/MoonJuYoungBlog"
repoId = "R_kgDORC6yYQ"
category = "General"
categoryId = "DIC_kwDORC6yYc4Cmq_5"
mapping = "pathname"
reactionsEnabled = "1"
emitMetadata = "0"
inputPosition = "top"
theme = "preferred_color_scheme"
lang = "ko"
loading = "lazy"
```

#### 댓글 비활성화

**전체 비활성화**: `hugo.toml`에서 `comments = false`로 설정

**특정 글만 비활성화**: Front Matter에 추가

```yaml
---
title: "댓글 없는 글"
disableComments: true
---
```

#### 댓글 테마 변경

다크모드/라이트모드 자동 전환:
```toml
theme = "preferred_color_scheme"  # 현재 설정 (권장)
```

고정 테마:
```toml
theme = "light"        # 라이트 모드 고정
theme = "dark"         # 다크 모드 고정
theme = "dark_dimmed"  # 어두운 회색
```

#### 댓글 위치 변경

```toml
inputPosition = "top"     # 입력창 상단 (현재 설정)
inputPosition = "bottom"  # 입력창 하단
```

#### 댓글 관리

- 댓글은 GitHub Discussions에 저장됩니다
- [Discussions 탭](https://github.com/answndud/MoonJuYoungBlog/discussions)에서 관리 가능
- 스팸 댓글 삭제, 수정 등 GitHub에서 직접 관리

---

## 문제 해결

### 자주 발생하는 오류

#### 1. "YAML parsing error"

Front Matter 문법 오류입니다.

```yaml
# 잘못된 예
title: My Post: Subtitle  # 콜론 문제

# 올바른 예
title: "My Post: Subtitle"  # 따옴표로 감싸기
```

#### 2. 이미지가 표시되지 않음

- 경로 확인: `/images/...`로 시작해야 함
- 파일명 대소문자 확인 (Linux는 대소문자 구분)
- 파일이 `static/` 폴더에 있는지 확인

#### 3. 글이 보이지 않음

```yaml
draft: false  # true가 아닌지 확인
date: 2026-01-28  # 미래 날짜가 아닌지 확인
```

#### 4. 한글 깨짐

파일 인코딩이 UTF-8인지 확인하세요.

#### 5. 로컬과 배포 결과가 다름

```bash
# 로컬에서 production 환경으로 테스트
hugo server --environment production
```

---

## 체크리스트

### 새 글 발행 전

- [ ] 제목이 명확하고 키워드 포함
- [ ] description 작성 완료
- [ ] 적절한 태그/카테고리 설정
- [ ] 이미지 Alt 텍스트 작성
- [ ] draft: false 확인
- [ ] 로컬에서 미리보기 확인
- [ ] 맞춤법 검사

### 정기 점검

- [ ] Google Search Console 색인 상태 확인
- [ ] 깨진 링크 확인
- [ ] 이미지 최적화 상태
- [ ] 테마 업데이트 확인

---

## 참고 자료

- [Hugo 공식 문서](https://gohugo.io/documentation/)
- [PaperMod 테마 Wiki](https://github.com/adityatelange/hugo-PaperMod/wiki)
- [마크다운 가이드](https://www.markdownguide.org/)
- [Google SEO 가이드](https://developers.google.com/search/docs/fundamentals/seo-starter-guide)
