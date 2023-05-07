name: "🔍오탈자 또는 내용 수정/변경"
description: 번역된 문서에 수정/변경이 필요하다고 생각하실 때 🤔
title: "🔍[개선] <title>"
labels: ["번역 개선"]
assignees: [""]
body:
- type: dropdown
  id: license-agreement
  attributes:
    label: "라이선스 동의"
    description: |
      기여해주시는 내용에 BSD 3항 라이선스가 적용됨을 동의해주셔야 합니다.
      자세한 내용은 [기여하기 문서](https://github.com/PyTorchKorea/tutorials-kr/blob/master/CONTRIBUTING.md)를 참고해주세요.
      기여하기 문서를 확인하였으며, 본 PR 내용에 BSD 3항 라이선스가 적용됨에 동의합니다.
    multiple: false
    options:
      - 예, 본 PR에 BSD 3항 라이선스 적용에 동의합니다.
      - 아니오, 본 PR에 라이선스 적용에 동의하지 않습니다.
  validations:
    required: true
- type: input
  id: relate-issue
  attributes:
    label: "관련 이슈"
    description: |
      이 Pull Request와 관련있는 이슈 번호를 적어주세요.
      이슈 또는 PR 번호 앞에 #을 붙이시면 제목을 바로 확인하실 수 있습니다. (예. #999 )
    value: "#"
  validations:
    required: true
- type: dropdown
  id: pull-request-type
  attributes:
    label: "PR 종류"
    description: |
      기여해주시는 내용에 따라 어떠한 것들이 변경되는지 선택해주세요.
      필요 시 2개 이상 선택하실 수 있습니다.
    multiple: false
    options:
      - 오탈자를 수정하거나 번역을 개선하는 기여
      - 번역되지 않은 튜토리얼을 번역하는 기여
      - 공식 튜토리얼 내용을 반영하는 기여
      - 위 종류에 포함되지 않는 기여
  validations:
    required: true
- type: textarea
  id: description-to-be
  attributes:
    label: " PR 설명"
    description: |
      (필요하다면) 이 PR로 무엇이 달라지는지 대략적으로 알려주세요.
    placeholder: |
      예시) '잘못된 ㄱㄴㄷㄹ을 ㅁㅂㅅㅇ으로 변경합니다.'
  validations:
    required: false
