# ERP Analytics Design System

> 레퍼런스: https://erp-five-lemon.vercel.app/

## 개요

Nike-like 미니멀 UI · 흑백 중심 · 각진 카드 · Chart.js 차트

## 색상

| 토큰 | Hex | 용도 |
|------|-----|------|
| canvas | #ffffff | 배경 |
| ink | #111111 | 본문·CTA·히어로 |
| charcoal | #39393b | 본문 |
| mute | #707072 | 보조 텍스트 |
| cloud | #f5f5f5 | KPI·테이블 헤더 |
| hairline | #cacacb | 테두리 |
| success | #007d48 | 성공 |
| warn | #a66400 | 경고 |
| sale | #d30005 | PDF 버튼·오류 |
| info | #1151ff | 정보 |

## 타이포

- 본문: Inter
- 디스플레이: Bebas Neue
- KPI 숫자: tabular-nums

## 레이아웃

```
[Header: ERP ANALYTICS + 4탭 nav]
[Main: max-width 80rem]
  - 데이터 입력 (히어로 + 업로드 + 4상태 + 샘플 + 3단계)
  - 대시보드 (KPI 12 + 차트 8 + 테이블 3)
  - 분석보고서 (PDF 다운로드)
  - 원본 데이터
[Footer]
```

## 컴포넌트

- `nk-card`: 1px border, radius 0
- `nk-btn-primary/secondary/success/sale`: pill 버튼
- `kpi-grid`: 2→3→4열 반응형
- `chart-wrap`: height 16rem

## 차트 (Chart.js)

1. 월별 매출 추이 (Line)
2. 카테고리별 매출 (Bar)
3. 채널별 매출 (Bar)
4. 고객 등급별 매출 (Bar)
5. 결제수단별 (Pie)
6. 주문 상태 (Pie)
7. 브랜드 TOP (Horizontal Bar)
8. 지역 TOP (Horizontal Bar)
