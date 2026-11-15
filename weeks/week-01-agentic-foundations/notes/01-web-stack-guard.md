# web-stack-guard 제작과 검증

## 한 일

`web-stack-guard` 스킬을 만들고, 이 PC의 Codex와 Claude Code가 전역 설정에서 불러올 수 있도록 등록했다. 이후 `/Users/june/Repository/web-stack-guard-test`에서 스킬을 적용해 프론트엔드와 백엔드를 생성하고 구조 검증 테스트까지 실행했다.

## 스킬이 확인하는 기준

| 영역 | 기준 | 검증 방식 |
| --- | --- | --- |
| 백엔드 | Kotlin, Spring Boot, Gradle | 설정·구조·Gradle 테스트 |
| 프론트엔드 | React, TanStack, Bun | 설정·구조·Bun 테스트 |
| 구조 | DDD와 SOLID 원칙 | 모듈 경계와 의존 방향 확인 |
| 아키텍처 테스트 | ArchUnit, ArchUnitTS(`archunit`) | 실제 테스트 실행 |

## 확인한 결과

- Codex와 Claude Code에서 전역 스킬을 불러올 수 있도록 구성했다.
- 샘플 프로젝트에 프론트엔드와 백엔드를 생성했다.
- 백엔드의 Gradle 기반 ArchUnit 테스트와 프론트엔드의 Bun 기반 ArchUnitTS 테스트를 실제 실행해 스킬의 검증 흐름을 확인했다.

## 기록 범위

이 문서는 1주차 실습의 결과를 요약한 것이다. 각 프로젝트에 스킬을 적용할 때의 충족·누락 판정은 해당 프로젝트의 코드·설정·테스트 결과를 근거로 별도로 남긴다.
