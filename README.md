# MGT_Analytics Hub 📊

데이터 분석을 위한 통합 대시보드 플랫폼

## 📁 파일 구조

```
MGT_Analytics_Hub/
├── index.html                              # 메인 대시보드
└── tools/                                  # 분석 도구들
    ├── revenue_analytics.html              # 피벗 테이블 분석
    ├── paying_retention_analytics.html     # 리텐션 분석
    ├── contents_metadata_analytics.html    # 이미지 메타 분석
    └── metadata_pattern_analytics.html     # 메타데이터 패턴 분석
```

## 🚀 사용 방법

### GitHub Pages 배포

1. **새 Repository 생성**
   - Repository 이름: `mgt-analytics-hub` (또는 원하는 이름)
   - Public으로 설정

2. **파일 업로드**
   ```bash
   # 로컬에서 작업하는 경우
   git clone [your-repo-url]
   cd mgt-analytics-hub
   
   # index.html과 tools 폴더를 복사
   # 그리고 커밋
   git add .
   git commit -m "Initial commit: MGT Analytics Hub"
   git push origin main
   ```

3. **GitHub Pages 활성화**
   - Repository Settings → Pages
   - Source: Deploy from a branch
   - Branch: main, folder: / (root)
   - Save

4. **접속**
   - `https://[your-username].github.io/mgt-analytics-hub/`

### 로컬에서 테스트

```bash
# Python 3 사용
python -m http.server 8000

# 브라우저에서 접속
http://localhost:8000
```

## 🎨 디자인 특징

- **LNB**: 카키색 그라데이션 (khaki-olive tone)
- **메인**: 화이트 기반 클린 디자인
- **가독성**: 명확한 텍스트 색상 구분
- **반응형**: 모바일/태블릿 지원

## 🔧 각 도구 설명

### 1. 피벗 테이블 분석 📈
- 인터랙티브 피벗 테이블
- 다중 파일 업로드
- AI 기반 인사이트 (Groq API)
- CSV, XLSX 지원

### 2. 리텐션 분석 👥
- 결제 유저 리텐션 분석
- Daily/Weekly/Monthly 코호트
- 히트맵 시각화
- Google Sheets 연동

### 3. 이미지 메타 분석 🖼️
- 이미지 메타데이터 자동 추출
- 배치 프로세싱
- Google Gemini API 연동
- 태그 시스템

### 4. 메타데이터 패턴 분석 📊
- 콘텐츠 패턴 분석
- AI 기반 인사이트
- PDF 리포트 생성
- 다중 차트 시각화

## ⚙️ API 설정

일부 도구는 API 키가 필요합니다:

- **Gemini API**: 메타데이터 분석, 이미지 분석
- **Groq API**: 피벗 테이블 AI 인사이트
- **Google Sheets API**: 리텐션 분석

각 도구 내에서 API 키를 입력할 수 있습니다.

## 🎯 주요 기능

✅ **iframe 기반 격리**: 각 도구가 독립적으로 작동  
✅ **기존 코드 100% 보존**: 원본 HTML 수정 없음  
✅ **빠른 전환**: LNB 클릭으로 즉시 전환  
✅ **로딩 인디케이터**: 부드러운 사용자 경험  
✅ **검색 기능**: 향후 확장 가능  

## 🐛 문제 해결

### iframe이 안 보여요
- 파일 경로 확인: `tools/` 폴더가 있는지 체크
- 브라우저 콘솔 확인: F12 → Console 탭

### API가 안 돼요
- 각 도구 내에서 API 키 재설정
- 네트워크 연결 확인
- API 사용량 한도 확인

### 로컬에서 안 열려요
- 직접 HTML 파일 열기 대신 웹 서버 사용 필수
- `python -m http.server` 또는 VS Code Live Server

## 📝 향후 개선 사항

- [ ] 대시보드 메인 페이지 (요약 위젯)
- [ ] 도구별 레이아웃 최적화 (그리드 배치)
- [ ] 다크 모드
- [ ] 데이터 공유 기능
- [ ] 즐겨찾기/최근 사용 도구

## 👤 제작자

**우엉 (MGT)**  
Data Analyst | Tool Builder

---

**버전**: 1.0.0  
**마지막 업데이트**: 2024-11-24
