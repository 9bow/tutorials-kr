name: "🔍오탈자 또는 내용 수정/변경"
description: 번역된 문서에 수정/변경이 필요하다고 생각하실 때 🤔
title: "🔍[개선] <title>"
labels: ["번역 개선"]
assignees: [""]
body:
- type: input
  id: document-url
  attributes:
    label: "개선이 필요한 문서 URL"
    description: |
      수정이 필요한 URL을 남겨주세요.
      예. https://tutorials.pytorch.kr/beginner/basics/intro.html
    placeholder: |
      https://tutorials.pytorch.kr/beginner/basics/intro.html
  validations:
    required: true
- type: textarea
  id: description-as-is
  attributes:
    label: "수정/변경이 필요한 부분"
    description: |
      어떤 단어 / 문장 / 내용에 변경이 필요하다고 생각하세요?
    placeholder: |
      예시) 'ㄱㄴㄷㄹ은 문법적으로 잘못된 내용입니다.'
  validations:
    required: true
- type: textarea
  id: description-to-be
  attributes:
    label: "수정/변경이 되어야 할 내용"
    description: |
      위의 내용이 어떻게 수정 / 변경되어야 한다고 생각하세요?
    placeholder: |
      예시) 'ㄱㄴㄷㄹ 대신 ㅁㅂㅅㅇ을 사용해야 합니다.'
  validations:
    required: true
- type: textarea
  id: other-infomation
  attributes:
    label: "추가 정보"
    description: |
      위와 같이 생각하신 이유 또는 다른 참고할 정보가 있다면 알려주세요.
    placeholder: |
      예시)
      'ㅇㅇㅇㅇ에서는 ㄱㄴㄷㄹ 대신 ㅁㅂㅅㅇ 사용을 권장하고 있습니다.
      이 내용은 https://tutorials.pytorch.kr/beginner/basics/intro.html 에서 확인할 수 있습니다.'
    tip: |
      이미지 파일 또는 로그 파일 등을 끌어다 놓거나 붙여넣기하여 업로드/첨부할 수 있습니다.
  validations:
    required: false
