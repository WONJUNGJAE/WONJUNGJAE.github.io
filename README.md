# Knights Frontier 3기 블로그 시작 파일

별도 프로그램 설치 없이 GitHub Pages와 Jekyll로 작동하는 블로그입니다.

## 1. 업로드

1. GitHub에서 `내GitHub아이디.github.io`라는 **Public** 저장소를 만듭니다.
2. **Add file → Upload files**로 이동합니다.
3. ZIP을 압축 해제하고, **안쪽의 파일과 폴더 전체**를 드래그해서 올립니다. ZIP 자체는 업로드하지 않습니다.
4. Commit changes를 누릅니다.
5. 저장소 **Settings → Pages → Build and deployment**에서 `Deploy from a branch`, `main`, `/(root)`를 선택하고 Save를 누릅니다.
6. `https://내GitHub아이디.github.io`에서 결과를 확인합니다. 처음 배포되는 데 몇 분 걸릴 수 있습니다.

## 2. 자기소개 수정

- `_config.yml`: `title`, `author`, `description`, `welcome`, `github_username`를 수정합니다.
- `about.md`: 자기소개와 관심 분야를 수정합니다.
- `assets/css/style.css`: 색상이나 디자인을 수정할 수 있습니다. 특히 `:root`의 `--accent`는 강조 색상입니다.

## 3. 새 글 작성

저장소 → Add file → Create new file → 아래처럼 파일 이름을 입력합니다:

    _posts/2026-10-31-my-first-ctf.md

내용 예시:

```markdown
---
layout: post
title: "첫 번째 CTF 풀이 기록"
date: 2026-10-31 09:00:00 +0900
categories: [ctf]
description: "문제 풀이 과정에서 배운 내용을 복습합니다."
---

## 문제 개요

여기에 내용 작성

## 접근 방법

여기에 풀이 과정 작성

## 배운 점

여기에 정리
```

Commit changes 후 자동으로 블로그에 글이 추가됩니다.

카테고리 값은 아래 중 하나를 사용하세요.

| 보이는 이름 | categories 값 |
|---|---|
| 개발 | `development` |
| CTF/Wargame | `ctf` |
| Bug Bounty | `bug-bounty` |
| 블로그/기술문서 | `tech-docs` |
| 논문/컨퍼런스 | `research` |
| 공모전/자격증 | `experience` |

하나의 글을 두 카테고리에 놓고 싶으면 `categories: [development, ctf]`처럼 작성해도 됩니다.

## 주의할 점

- 글 파일명은 `_posts/연도-월-일-영어제목.md` 형태로 만드세요.
- `_posts`, `_layouts`, `_config.yml`의 밑줄은 필수입니다.
- Jekyll에서 미래 날짜의 글은 표시되지 않을 수 있습니다.
- GitHub Pages URL이 `https://아이디.github.io`가 아니라 프로젝트 경로 아래라면 `_config.yml`의 `baseurl` 변경이 필요할 수 있습니다.
- HTML/Markdown/YAML 파일을 수동 편집하여 운영하는 스타터이며 회원 로그인, 댓글, 검색 기능은 포함되지 않습니다.
