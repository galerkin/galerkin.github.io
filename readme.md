# galerkin.github.io

이 저장소는 [Hugo](https://gohugo.io/)와 Bear 테마를 사용하여 구축된 정적 블로그/이력서 사이트입니다. GitHub Actions를 통해 자동으로 빌드 및 GitHub Pages(https://galerkin.github.io)로 배포됩니다.

## 주요 특징
- **Hugo**: 빠르고 유연한 정적 사이트 생성기
- **Bear 테마**: 심플하고 미니멀한 블로그 테마
- **GitHub Actions**: 자동 빌드 및 배포 파이프라인
- **블로그/이력서/소개 페이지**: content 디렉토리에서 관리

## 로컬 개발 방법
```sh
cd hugo-site
hugo server -D
```
- http://localhost:1313 에서 사이트를 미리 볼 수 있습니다.

## 배포 방법
- main 브랜치에 push하면 GitHub Actions가 자동으로 빌드 및 gh-pages 브랜치로 배포합니다.
- 커스텀 도메인(CNAME): galerkin.github.io

## 디렉토리 구조
- `hugo-site/` : Hugo 프로젝트 루트
  - `content/` : 페이지 및 블로그 글
  - `themes/hugo-bearblog/` : Bear 테마

## 참고
- `.github/workflows/gh-pages.yml` : GitHub Actions 워크플로우 파일

# run locally
```bash
hugo server
```
