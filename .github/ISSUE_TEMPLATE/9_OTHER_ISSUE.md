name: "📃기타 다른 이슈"
description: 위 이슈들이 아닌 다른 이슈들을 남기실 때 📬
title: "📃[기타] <title>"
labels: ["기타 이슈"]
assignees: [""]
body:
- type: textarea
  id: description-as-is
  attributes:
    label: "이슈 내용"
    description: |
      어떤 이슈인지 알려주세요.
    placeholder: |
      새로운 PyTorch 버전이 릴리즈되어, 버전 업데이트가 필요합니다.
  validations:
    required: true
- type: textarea
  id: other-infomation
  attributes:
    label: "추가 정보"
    description: |
      다른 참고할 정보 또는 URL 등이 있다면 알려주세요.
    placeholder: |
      예시) https://pytorch.kr/get-started/pytorch-2.0/
    tip: |
      이미지 파일 또는 로그 파일 등을 끌어다 놓거나 붙여넣기하여 업로드/첨부할 수 있습니다.
  validations:
    required: false
