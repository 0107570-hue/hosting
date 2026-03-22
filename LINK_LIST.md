# 맞춤 제안서 배포 링크 목록

> **용도**: 클라이언트에게 공유 가능한 배포 URL 관리  
> **관리**: 제안서 생성 완료 후 자동 업데이트  
> **보관**: GitHub hosting 저장소 (단일 원본)

---

## 📋 제안서 링크 목록

| # | 클라이언트명 | 회사/업종 | 배포 URL | 생성일 | 발송일 | 피드백 |
|---|-----------|---------|---------|-------|-------|-------|
| 1 | 인천청라골프연습장 | 인도 골프연습장 | [링크](https://hosting-rose-phi.vercel.app/proposals/인천청라골프연습장_proposal.html) | 2026-03-22 | - | - |

---

## 📌 사용 규칙

### 추가 방법
새 제안서 생성 시:
1. 검수/확정 완료 후 `proposals/` 폴더에 HTML 저장
2. GitHub 푸시 
3. 아래 테이블에 행(행) 추가
4. 클라이언트 이름, 회사/업종, 배포 URL, 생성일 기입
5. 발송 후 "발송일" 체크

### 링크 형식
```
[링크](https://hosting-rose-phi.vercel.app/proposals/파일명.html)
```

### 삭제 원칙
- 로컬 `proposal1/` 폴더의 작업본은 배포 후 삭제 (선택)
- GitHub `hosting/proposals/` 폴더의 원본은 **삭제 금지** (이력 보관)
- 이 링크 목록(LINK_LIST.md)은 계속 누적 관리

---

## 🔄 배포 플로우

```
1. 로컬 작업 (proposal1/)
   ├─ 클라이언트 정보 파일 생성
   ├─ HTML 제안서 작성/검수
   └─ 최종 검수 완료

2. GitHub 푸시 (hosting/)
   ├─ proposals/파일명.html 저장
   ├─ 자동 Vercel 배포
   └─ 배포 URL 생성

3. 링크 목록 업데이트 (LINK_LIST.md)
   ├─ 새 행 추가
   ├─ URL 기입
   └─ GitHub 푸시

4. 클라이언트 공유
   ├─ 이 파일의 URL만 공유
   └─ 제안서 열람 (클라이언트)
```

---

## 💾 저장된 파일 위치

| 항목 | 로컬 | GitHub | 설명 |
|------|------|--------|------|
| **작업본 HTML** | `proposal1/` | ❌ | 작업 완료 후 선택 삭제 |
| **원본 HTML** | ❌ | `hosting/proposals/` | ✅ 영구 보관 |
| **이미지 자산** | ❌ | `hosting/images/` | 이미지 필요시 업로드 |
| **링크 목록** | ❌ | `hosting/LINK_LIST.md` | ✅ 이 파일 (누적 관리) |

---

## 🌐 배포 기본 설정

- **Vercel 도메인**: https://hosting-rose-phi.vercel.app
- **GitHub 저장소**: https://github.com/0107570-hue/hosting
- **자동 배포**: GitHub push → Vercel (즉시 반영)
- **프로포절 경로**: `/proposals/파일명.html`
- **이미지 경로**: `/images/파일명.jpg` (필요시)

---

**최종 관리 담당**: 자동화 시스템  
**업데이트**: 매 제안서 배포 후 즉시  
**백업**: GitHub (모든 버전 이력 보관)
