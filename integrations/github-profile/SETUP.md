# 최신 글 카드 연결

1. 이 블로그의 변경 사항을 `gh-pages` 브랜치에 commit/push합니다.
2. GitHub Pages 배포가 끝나면 `https://dev.choijw1004.site/github/latest-1.svg`가 표시되는지 확인합니다.
3. 이 폴더의 `README.md` 내용을 `choijw1004/choijw1004` 저장소의 프로필 README에 한 번 붙여넣습니다.

이후 블로그에 푸시하여 GitHub Pages가 배포될 때마다 Jekyll이 `site.posts`에서 최신 글 3개를 읽어 SVG 카드를 다시 만듭니다. 프로필 README의 Markdown과 이미지 주소는 그대로 사용합니다. 별도 워크플로, 토큰, 프로필 자동 커밋은 필요하지 않습니다.

카드 링크도 고정 주소를 사용합니다. `/github/latest-1/`, `/github/latest-2/`, `/github/latest-3/`가 각각 현재 첫 번째, 두 번째, 세 번째 최신 글로 이동하므로 새 글을 올려도 링크를 수정할 필요가 없습니다.

GitHub는 외부 이미지를 캐시하므로 배포 직후 프로필 이미지 갱신은 지연될 수 있습니다. 이 경우 갱신 전 제목이 잠시 보일 수 있으며, 클릭하면 배포된 현재 순위의 글로 이동합니다.

관련 문서: [Jekyll 글 목록](https://jekyllrb.com/docs/variables/), [GitHub 이미지 캐시](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/about-anonymized-urls).
