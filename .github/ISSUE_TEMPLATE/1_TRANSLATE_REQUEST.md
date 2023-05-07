name: "📖번역 진행 / 요청"
description: 번역을 진행하실 문서가 있거나 번역을 요청하실 때 📝
title: "📖[번역] <title>"
labels: ["번역 요청"]
assignees: [""]
body:
- type: input
  id: document-url
  attributes:
    label: "번역이 필요한 문서 URL"
    description: 번역을 하실 / 요청하실 URL을 남겨주세요.
    placeholder: ex. https://tutorials.pytorch.kr/beginner/basics/intro.html
  validations:
    required: true
- type: dropdown
  id: request-to
  attributes:
    label: "직접 번역 여부"
    description: 직접 번역을 하시거나, 다른 분에게 번역을 요청하실 수 있습니다.
    multiple: false
    options:
      - 예, 제가 진행하려고 합니다.
      - 아니오, 다른 분께 요청드립니다.
  validations:
    required: true
- type: textarea
  id: due-date
  attributes:
    label: "(직접 번역 시) 예상하는 완료 일정"
    description: 반드시 지키셔야 하는 일정이 아닙니다. 일정이 늦어질 경우 다른 번역자를 위해 남겨주세요.
    placeholder: "예시) 1달 후, 또는 3월 내 등'"
  validations:
    required: false
- type: input
  id: relate-issue
  attributes:
    label: "관련 이슈"
    description: 현재 번역 요청 / 진행 내역을 보기 위해 각 버전의 메인 이슈를 참조합니다.
    value: "#660 (v2.0)"
  validations:
    required: true
- type: textarea
  id: other-infomation
  attributes:
    label: "추가 정보"
    description: |
      다른 참고할 정보가 있다면 알려주세요.
    placeholder: |
      예시)
      'ㅇㅇㅇㅇ에서는 ㄱㄴㄷㄹ 대신 ㅁㅂㅅㅇ 사용을 권장하고 있습니다.
      이 내용은 https://tutorials.pytorch.kr/beginner/basics/intro.html 에서 확인할 수 있습니다.'
    tip: |
      이미지 파일 또는 로그 파일 등을 끌어다 놓거나 붙여넣기하여 업로드/첨부할 수 있습니다.
  validations:
    required: false
