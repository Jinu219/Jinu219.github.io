# PySDM Seeding Lab

`Jinu219.github.io`에서 공개되는 Quarto 기반 연구 블로그입니다. PySDM 학습 기록, 실험 환경 구축 과정, 구름 씨뿌리기 수치 실험을 한곳에 정리합니다.

## 로컬에서 확인하기

1. [Quarto](https://quarto.org/docs/get-started/)를 설치합니다.
2. 저장소 루트에서 `quarto preview`를 실행합니다.
3. 정적 결과만 만들려면 `quarto render`를 실행합니다.

빌드 결과인 `_site/`는 버전 관리에서 제외됩니다.

## 새 글 작성하기

`_templates/post/index.qmd`를 새 폴더에 복사해 시작합니다.

```text
posts/
  learn-pysdm/
  build-the-lab/
  experiments/
```

글에 사용하는 그림은 해당 글의 `images/` 폴더에 두고, 논문과 소프트웨어 인용은 루트의 `references.bib`에 추가합니다.

## 배포

`main` 브랜치에 푸시하면 GitHub Actions가 사이트를 렌더링하고 결과를 `gh-pages` 브랜치에 게시합니다. 최초 실행 후 저장소의 **Settings → Pages → Build and deployment**에서 소스를 `Deploy from a branch`, 브랜치를 `gh-pages`와 `/(root)`로 지정해야 합니다.
