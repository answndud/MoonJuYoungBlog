# GitHub Blog with Hugo

Hugo와 GitHub Pages를 사용한 개인 블로그입니다.

## 시작하기 전에

### 1. 설정 파일 수정

`hugo.toml` 파일에서 다음 항목들을 본인의 정보로 수정하세요:

- `baseURL`: `https://YOUR_USERNAME.github.io/` 형식으로 변경
- `params.author`: 본인 이름
- `params.description`: 블로그 설명
- `params.socialIcons`: GitHub URL과 이메일 주소
- `params.editPost.URL`: GitHub 저장소 URL

### 2. GitHub 저장소 생성

1. GitHub에서 `USERNAME.github.io` 이름의 새 저장소 생성 (USERNAME은 본인의 GitHub 아이디)
2. 또는 다른 이름의 저장소를 생성할 수도 있습니다

### 3. 원격 저장소 연결 및 푸시

```bash
git remote add origin https://github.com/USERNAME/USERNAME.github.io.git
git add .
git commit -m "Initial commit: Hugo blog setup"
git push -u origin main
```

### 4. GitHub Pages 설정

1. GitHub 저장소의 **Settings** → **Pages** 이동
2. **Source**를 **GitHub Actions**로 선택
3. 자동으로 배포가 시작됩니다

## 로컬에서 블로그 실행

```bash
hugo server -D
```

브라우저에서 `http://localhost:1313` 접속

## 새 포스트 작성

```bash
hugo new posts/my-new-post.md
```

또는 `content/posts/` 폴더에 직접 마크다운 파일을 생성하세요.

### 포스트 템플릿

```markdown
---
title: "포스트 제목"
date: 2026-01-28
draft: false
tags: ["태그1", "태그2"]
categories: ["카테고리"]
description: "포스트 설명"
---

본문 내용...
```

- `draft: true`로 설정하면 배포 시 포함되지 않습니다
- `hugo server -D` 옵션으로 draft 포스트도 미리보기 가능

## 테마 커스터마이징

[PaperMod 테마 문서](https://github.com/adityatelange/hugo-PaperMod/wiki)를 참고하세요.

## 디렉토리 구조

```
.
├── archetypes/        # 콘텐츠 템플릿
├── content/           # 블로그 콘텐츠
│   ├── posts/         # 블로그 포스트
│   ├── archives.md    # 아카이브 페이지
│   └── search.md      # 검색 페이지
├── themes/            # Hugo 테마
│   └── PaperMod/
├── .github/
│   └── workflows/     # GitHub Actions 워크플로우
├── hugo.toml          # Hugo 설정 파일
└── README.md
```
