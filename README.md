# ERP 분석 대시보드

[레퍼런스](https://erp-five-lemon.vercel.app/) 구조를 따른 **단일 HTML** ERP 대시보드입니다.

## 폴더 구성

```
0612실습_dashboard/
├── index.html          ← 메인 앱 (이 파일을 열면 됨)
├── products.csv        ← 샘플 데이터
├── customers.csv
├── sales_orders.csv
├── sales_order_items.csv
├── DESIGN.md
└── README.md
```

## 로컬 실행

CSV 샘플 로드는 **웹 서버**가 필요합니다 (파일 더블클릭 `file://` 은 샘플 fetch 불가).

```powershell
cd "c:\Users\skku\Desktop\0612실습_dashboard"
npx --yes serve .
```

브라우저에서 `http://localhost:3000` 접속 → **샘플 데이터 불러오기** → **대시보드**

## Vercel 배포 (새 프로젝트)

1. GitHub에 **새 저장소** 생성 후 이 폴더 업로드
2. [vercel.com](https://vercel.com) → **Add New Project** → 저장소 선택
3. Framework: **Other** (빌드 명령 없음)
4. Deploy → `https://프로젝트명.vercel.app` 로 접속

## 기능

- CSV 4종 업로드 (최대 4건) + 검증 + 에러 메시지
- KPI 12개 + Chart.js 차트 8종
- 분석보고서 + PDF 다운로드
- 원본 데이터 미리보기

## CSV 파일

| 파일 | 설명 |
|------|------|
| products.csv | 상품 |
| customers.csv | 고객 |
| sales_orders.csv | 주문 |
| sales_order_items.csv | 주문상세 |
