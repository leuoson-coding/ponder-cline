# Ponder

Ponder에 기여하는 것에 관심을 가져주셔서 감사합니다! 버그 수정, 기능 추가, 문서 개선 등 모든 기여는 Ponder을 더욱 스마트하게 만드는 데 기여합니다. 활기차고 환영하는 커뮤니티를 유지하기 위해 모든 구성원은 [행동 강령](CODE_OF_CONDUCT.md)을 준수해야 합니다.

## 버그와 문제 보고

버그 보고는 Ponder을 모두에게 더 나은 것으로 만드는 데 도움이 됩니다! 새로운 이슈를 생성하기 전에, 중복을 피하기 위해 [기존 이슈를 검색](https://github.com/leuoson/ponder/issues)해 주세요. 버그를 보고할 준비가 되었다면, [이슈 페이지](https://github.com/leuoson/ponder/issues/new/choose)로 이동하여 관련 정보를 작성하기 위한 템플릿을 사용해 주세요.

<blockquote class='warning-note'>
    🔐 <b>중요:</b> 보안 취약점을 발견한 경우, <a href="https://github.com/leuoson/ponder/security/advisories/new">GitHub 보안 도구를 사용하여 비공개로 보고</a>해 주세요.
</blockquote>

## 작업 내용 결정하기

첫 기여를 찾고 계신가요? ["good first issue"](https://github.com/leuoson/ponder/labels/good%20first%20issue)나 ["help wanted"](https://github.com/leuoson/ponder/labels/help%20wanted) 라벨이 붙은 이슈를 확인해 보세요. 이러한 이슈들은 새로운 기여자를 위해 특별히 선정된 작업으로, 도움이 필요한 영역이 표시되어 있습니다!

또한, [문서](https://github.com/leuoson/ponder/tree/main/docs)에 대한 기여도 환영합니다! 오타 수정, 기존 가이드 개선, 새로운 교육 콘텐츠 작성 등, 커뮤니티 주도의 리소스 저장소를 구축하는 데 여러분의 도움이 필요합니다. `/docs`를 살펴보고 개선이 필요한 부분을 찾아보세요.

큰 기능에 대해 작업할 계획이 있다면, 먼저 [기능 요청](https://github.com/leuoson/ponder/discussions/categories/feature-requests?discussions_q=is%3Aopen+category%3A%22Feature+Requests%22+sort%3Atop)을 생성하여 이것이 Ponder의 비전과 부합하는지 논의하는 것이 좋습니다.

## 개발 환경 설정

1. **VS Code 확장 프로그램**

    - 프로젝트를 열면 VS Code가 권장 확장 프로그램 설치를 안내합니다
    - 개발을 위해 이 확장 프로그램들이 필요하므로, 설치 안내를 수락해 주세요.
    - 프롬프트를 닫은 경우 확장 프로그램 패널에서 수동으로 설치할 수 있습니다

2. **로컬 개발**
    - `npm run install:all`을 실행하여 의존성을 설치합니다
    - `npm run test`를 실행하여 로컬에서 테스트를 실행합니다
    - PR을 제출하기 전에 `npm run format:fix`를 실행하여 코드를 포맷팅합니다

## 코드 작성과 제출

누구나 Ponder에 코드를 기여할 수 있지만, 기여가 원활하게 통합되도록 다음 가이드라인을 따라주세요:

1. **Pull Request 집중하기**

    - PR은 단일 기능 또는 버그 수정으로 제한해 주세요
    - 큰 변경사항은 작은 관련 PR로 분할해 주세요
    - 논리적으로 독립적인 커밋 단위로 나누어 리뷰가 용이하도록 구성하세요.

2. **코드 품질**

    - `npm run lint`를 실행하여 코드 스타일을 체크합니다
    - `npm run format`을 실행하여 코드를 자동으로 포맷팅합니다
    - 모든 PR은 린팅과 포맷팅을 포함한 CI 체크를 통과해야 합니다
    - 제출 전에 ESLint 경고나 에러를 모두 해결해 주세요
    - TypeScript 모범 사례를 따르고, 타입 안전성을 유지해 주세요

3. **테스트**

    - 새로운 기능에는 테스트를 추가해 주세요
    - `npm test`를 실행하여 모든 테스트가 통과하는지 확인해 주세요
    - 변경사항이 기존 테스트에 영향을 미치는 경우 해당 테스트를 업데이트해 주세요
    - 적절한 경우 단위 테스트와 통합 테스트를 모두 포함해 주세요

4. **Changesets를 활용한 버전 관리**

    - 사용자에게 영향을 미치는 변경 사항이 있는 경우, `npm run changeset`을 실행하여 changeset을 생성해 주세요
    - 적절한 버전 증가 옵션을 선택하세요:
        - `major` 호환되지 않는 변경 (1.0.0 → 2.0.0)
        - `minor` 새로운 기능 추가 (1.0.0 → 1.1.0)
        - `patch` 버그 수정 (1.0.0 → 1.0.1)
    - 영향을 설명하는 명확한 변경사항 메시지를 작성해 주세요
    - 문서 변경만 있는 경우 changeset이 필요하지 않습니다

5. **커밋 가이드라인**

    - 명확하고 설명적인 커밋 메시지를 작성해 주세요
    - 컨벤셔널 커밋 형식(예: "feat:", "fix:", "docs:")을 사용해 주세요
    - 커밋에서 관련 이슈를 #issue-number를 사용하여 참조해 주세요

6. **제출 전 확인사항**

    - 최신 main에 브랜치를 리베이스해 주세요
    - 브랜치가 정상적으로 빌드되는지 확인해 주세요
    - 모든 테스트가 통과하는지 다시 확인해 주세요
    - 디버그 코드나 콘솔 로그가 없는지 변경사항을 확인해 주세요

7. **Pull Request 설명**
    - 변경 내용을 명확하게 설명해 주세요
    - 변경사항을 테스트하는 방법을 포함해 주세요
    - 호환되지 않는 변경 사항이 있다면 목록으로 작성해주세요
    - UI 변경이 있는 경우, 스크린샷을 추가해 주세요

## 기여 동의서

Pull Request를 제출함으로써, 귀하의 기여가 프로젝트와 동일한 라이선스([Apache 2.0](/LICENSE)) 에 따라 제공됨에 동의하는 것입니다.

기억하세요: Ponder에 기여하는 것은 코드를 작성하는 것뿐만 아니라, AI 지원 글쓰기의 미래를 형성하는 커뮤니티의 일원이 되는 것입니다. 함께 멋진 것을 만들어봅시다! 🚀
