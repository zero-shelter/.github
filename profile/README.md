# zero-shelter

Review dependency scanner findings, available upgrades, and changes since your last recorded run.

zero-shelter combines supported scanner reports, ranks findings using documented rules, and compares them with a baseline of accepted risks. Use the terminal or an HTML report, add the result to CI, or pass it to a coding agent. The tool runs locally without a runtime LLM; invoked scanners have their own network behavior.

[Website](https://zero-shelter.github.io) · [Source and documentation](https://github.com/zero-shelter/zero-shelter) · [npm package](https://www.npmjs.com/package/zero-shelter) · [Community discussions](https://github.com/zero-shelter/discussions/discussions)

  <p>
    <a href="https://zero-shelter.github.io">
      <img src="https://img.shields.io/badge/Website-zero--shelter.github.io-292929?labelColor=181717&amp;style=flat-square&amp;logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgc3Ryb2tlPSJ3aGl0ZSIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiPjxjaXJjbGUgY3g9IjEyIiBjeT0iMTIiIHI9IjEwIi8%2BPHBhdGggZD0iTTIgMTJoMjBNMTIgMmExOCAxOCAwIDAgMSAwIDIwIDE4IDE4IDAgMCAxIDAtMjAiLz48L3N2Zz4%3D&amp;logoColor=white" alt="Visit website" />
    </a>
    <a href="https://www.npmjs.com/package/zero-shelter">
      <img src="https://img.shields.io/npm/v/zero-shelter?style=flat-square&amp;logo=npm&amp;logoColor=white&amp;label=npm&amp;labelColor=181717&amp;color=292929" alt="npm version" />
    </a>
    <br />
    <a href="https://www.npmjs.com/package/zero-shelter">
      <img src="https://img.shields.io/npm/dy/zero-shelter?style=flat-square&amp;logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgc3Ryb2tlPSJ3aGl0ZSIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiPjxwYXRoIGQ9Ik0yMSAxNXY0YTIgMiAwIDAgMS0yIDJINWEyIDIgMCAwIDEtMi0ydi00TTcgMTBsNSA1IDUtNU0xMiAxNVYzIi8%2BPC9zdmc%2B&amp;label=Downloads&amp;labelColor=181717&amp;color=292929" alt="npm downloads in the last 365 days" />
    </a>
    <a href="https://www.npmjs.com/package/zero-shelter">
      <img src="https://img.shields.io/npm/last-update/zero-shelter/latest?style=flat-square&amp;logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgc3Ryb2tlPSJ3aGl0ZSIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiPjxyZWN0IHg9IjMiIHk9IjUiIHdpZHRoPSIxOCIgaGVpZ2h0PSIxNiIgcng9IjIiLz48cGF0aCBkPSJNMTYgM3Y0TTggM3Y0TTMgMTFoMThNOCAxNmgyTTE0IDE2aDIiLz48L3N2Zz4%3D&amp;label=Released&amp;labelColor=181717&amp;color=292929" alt="Latest npm version publish date" />
    </a>
  </p>

```sh
npx zero-shelter judge
```

Requires Node.js 20 or later and a supported project or saved scanner report. See the [installation guide](https://github.com/zero-shelter/zero-shelter#install) for scanner setup. The package is a preview; release notes describe the available features and compatibility changes.

The current tool covers dependency findings. A run with no new findings does not establish that the project is secure, and accepting a finding does not fix it.

Maintained by [@hadevyi](https://github.com/hadevyi), [@PresentJay](https://github.com/PresentJay), and [@msnodeve](https://github.com/msnodeve), with [contributions from the community](https://github.com/zero-shelter/zero-shelter/graphs/contributors).

## 한국어

의존성 검사 결과와 가능한 업그레이드, 이전 실행 이후의 변화를 확인하는 도구입니다.

지원하는 스캐너의 결과를 합치고, 문서에 명시한 규칙으로 순위를 계산한 뒤 수용한 위험을 기록한 baseline과 비교합니다. 터미널·HTML 보고서에서 직접 확인하거나 CI·코딩 에이전트에 연결할 수 있습니다. 도구는 로컬에서 실행하며 런타임 LLM을 사용하지 않습니다. 실행하는 스캐너는 각자의 네트워크 동작을 따릅니다.

Node.js 20 이상과 지원하는 프로젝트 파일 또는 저장된 스캐너 보고서가 필요합니다. [한국어 설치 안내](https://github.com/zero-shelter/zero-shelter/blob/main/README.ko.md#설치)에서 설정 방법을 확인할 수 있습니다.

현재 프리뷰는 의존성 검사 결과를 다룹니다. 새 항목이 없다고 프로젝트가 안전하다는 뜻은 아니며, 위험을 수용해 기록해도 취약점이 수정되는 것은 아닙니다.
