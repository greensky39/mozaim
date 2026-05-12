# MOZA Landing Page Deployment Guide

## 1) Vercel 프로젝트 생성
1. https://vercel.com 접속 후 로그인
2. `Add New...` -> `Project`
3. Git 저장소 연결(또는 로컬에서 Vercel CLI 사용)
4. Framework Preset은 `Other`로 두고 Deploy

## 2) 도메인 연결 (moza.im)
1. Vercel 프로젝트 -> `Settings` -> `Domains`
2. `moza.im` 추가
3. `www.moza.im`도 추가

## 3) 후이즈 DNS 설정
Vercel에서 안내하는 값으로 DNS를 맞춤.
일반적으로 아래 중 하나를 사용:
- 루트 도메인(`@`): `A` 레코드 -> `76.76.21.21`
- `www`: `CNAME` -> `cname.vercel-dns.com`

## 4) SSL 확인
1. DNS 전파 후 Vercel Domains 화면에서 `Valid Configuration` 확인
2. HTTPS 인증서 자동 발급 완료 확인

## 5) 내용 확정 필요 항목
- `index.html`의 `사업자번호 (입력 예정)`을 실제 사업자번호로 교체

## 6) 수정 파일
- `index.html`
- `vercel.json`
