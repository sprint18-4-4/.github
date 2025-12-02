<img src="https://private-user-images.githubusercontent.com/169524126/521039880-a378be81-f539-4529-8701-5d3b4193c61a.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NjQ2Mjk3MjAsIm5iZiI6MTc2NDYyOTQyMCwicGF0aCI6Ii8xNjk1MjQxMjYvNTIxMDM5ODgwLWEzNzhiZTgxLWY1MzktNDUyOS04NzAxLTVkM2I0MTkzYzYxYS5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUxMjAxJTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MTIwMVQyMjUwMjBaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1iNmU5YWVjOTFhY2U5Nzk0ZTIzNWYyZjAzY2IwNjA3NjdmOTNlMWQ1YTExZTcxYzIwYjdjZTQyNTMzYzUzOTAwJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.df0yEL2wQ0DOsEMSjsRKCNr-O_5kLEBqfNDZMbkELZc" />

<p align="center">
  <a href="https://coworkers-chi.vercel.app/">배포 바로가기</a> ·
  <a href="https://github.com/sprint18-4-4/Coworkers">깃허브 바로가기</a>
</p>

## 1. 프로젝트 개요

Coworkers는 **팀의 일정·할 일을 한 화면에서 관리**하고,
반복 업무와 커뮤니케이션 부담을 줄여주는 협업용 웹 서비스입니다.

- 누구를 위한 서비스인가요?
  - 스타트업/사이드프로젝트 팀, 스터디 모임 등
- 어떤 문제를 해결하나요?
  - 팀 일정과 할 일이 칸반보드, 캘린더 등 여러 도구에 흩어져 관리되는 문제를 한 화면에서 정리합니다.
  - 정리된 일정·업무 내역은 필요 시 PDF로 내보내, 회의 자료나 보고용으로 바로 활용할 수 있습니다.

## 2. 핵심 시나리오

### 2-0. 랜딩 페이지

<img src="https://private-user-images.githubusercontent.com/169524126/521575126-2decf3c0-2c48-47bc-af36-b51d224fae91.gif?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NjQ3MTI3OTAsIm5iZiI6MTc2NDcxMjQ5MCwicGF0aCI6Ii8xNjk1MjQxMjYvNTIxNTc1MTI2LTJkZWNmM2MwLTJjNDgtNDdiYy1hZjM2LWI1MWQyMjRmYWU5MS5naWY_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUxMjAyJTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MTIwMlQyMTU0NTBaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT0yNmU1ODIwYzVjZmQyNjEwNjcwNjU1ZDQzM2MxMGNkNzRkOWY5YzZkYTJmNmFkYTQzMTI2MTdkMDk0ZmJlNTc0JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.LJGQ5IurQVKMEAVUGZTyHP5jGC16fWuggrp7NPyVadM" />

1. GSAP을 활용해 스크롤 기반 인터랙션을 구현했습니다.
2. 최초 가입 시 온보딩 모달을 통해 팀 생성·초대 흐름을 안내합니다.
3. ‘지금 시작하기’ 버튼 클릭 시 팀 페이지로 이동합니다.
   - 별도의 복잡한 설정 없이 바로 팀 보드/캘린더를 사용할 수 있습니다.

### 2-1. 팀 생성 및 일정 · 할 일 관리

<img src="https://private-user-images.githubusercontent.com/169524126/521575127-a0201b07-74d0-42d2-bea9-826e11cfb996.gif?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NjQ3MTI3OTAsIm5iZiI6MTc2NDcxMjQ5MCwicGF0aCI6Ii8xNjk1MjQxMjYvNTIxNTc1MTI3LWEwMjAxYjA3LTc0ZDAtNDJkMi1iZWE5LTgyNmUxMWNmYjk5Ni5naWY_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUxMjAyJTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MTIwMlQyMTU0NTBaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1jMzVlMWM0YzA3NTk3YTMwNzBjMmRjNzZkYmE4NmU3MTA4ZGMwZGJlMTIzOTM1MTVkMDJjY2UyYzI1MGRjOGZhJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.Fsk7FcmHlN22vRuMwLoOapuLD3uuSkVew9h6Zlw3yV0"/>

1. 팀을 생성하고 초대 링크로 멤버를 초대합니다.
2. 팀별 기본 보드와 캘린더가 자동으로 생성됩니다.
3. 날짜를 선택해 일정/할 일을 추가합니다.
4. 반복 주기(매일/매주/매월)를 설정해 반복 업무를 자동 생성합니다.
5. 마감일, 상태를 변경하며 진행 상황을 추적합니다.

### 2-2. 팀 게시판 (대시보드)

<img src="https://private-user-images.githubusercontent.com/169524126/521575125-fa8f5aa6-2b0c-4df2-b99b-fccc6570b2b5.gif?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NjQ3MTI3OTAsIm5iZiI6MTc2NDcxMjQ5MCwicGF0aCI6Ii8xNjk1MjQxMjYvNTIxNTc1MTI1LWZhOGY1YWE2LTJiMGMtNGRmMi1iOTliLWZjY2M2NTcwYjJiNS5naWY_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUxMjAyJTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MTIwMlQyMTU0NTBaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT05MjIyMzVhMWUwOTdlNjQxYWI4YTE1NmEyNDFhYmM5YjdmNWRmZTI4MTE4YzY3NWQ3MjFkNjlkY2Y1N2RjOGU5JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.YGVhBlPenoe9z2aEQuDtd34W8l_abh6NotoublCmf0Y" />

1. 팀원이 자유롭게 게시글을 작성할 수 있습니다.
2. 게시글은 팀원에게만 공개되며, 목록은 무한 스크롤로 제공됩니다.
3. 게시글 상세에서 댓글과 좋아요로 소통할 수 있습니다.

## 3. 주요 기능

- 온보딩 UI
  - 최초 로그인 시 온보딩 화면 제공
- 팀/그룹 관리
  - 팀 생성, 초대, 멤버 권한 관리
- 일정 · 할 일 관리
  - 반복 일정, 상태(할 일/진행 중/완료) 관리
- 댓글 및 메모
  - 할 일 단위 댓글 작성/수정/삭제
- PDF 내보내기
  - 할 일 내역을 PDF로 내보낼 수 있습니다.

## 4. 기술 스택 요약

자세한 기술 스택과 개발 환경은 [Frontend README](https://github.com/sprint18-4-4/Coworkers/blob/develop/README.md)에 정리되어 있습니다.

- **Framework**: Next.js 16 (App Router)
- **Language**: TypeScript
- **State Management**: React Query, Zustand
- **Styling**: Tailwind CSS
- **Animation**: Framer Motion, GSAP
- **문서화/테스트**: Storybook, Chromatic

<p align="right" style="margin-top: 5rem;">
  <small style="color:#6b7280;">
    코드잇 스프린트 프론트엔드 심화 프로젝트 (2025.01 ~ 2025.12)
  </small>
</p>
