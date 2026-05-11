# NAVIGATE Lab — Public Accuracy Ledger

**한국어 스마트머니 + AI 비전 인텔리전스의 시그널 정확도 공개 기록**

매일 KST 09:00 (월~토) Anthropic 클라우드 환경에서 자동 실행되는 `cloud_accuracy_ledger.py` routine이 `signal_log.parquet` 원본 데이터를 재계산하여 [`ACCURACY.md`](./ACCURACY.md)에 prepend합니다.

운영자가 사후 조작할 수 없는 구조입니다 — git history (immutable) + Anthropic 클라우드 sandbox (운영자 PC 분리) 이중 안전장치.

---

## 📊 검증 방법

1. [`ACCURACY.md`](./ACCURACY.md) 클릭 → 매일 추가되는 entry 확인
2. **git history** 클릭 → 모든 commit 시간 + diff 확인 가능
3. **commit author** = `cloud-routine[bot]` (운영자 계정과 분리)

---

## 📐 측정 방법론

- **Universe**: SPY · QQQ · DIA · KOSPI · KOSDAQ (5개 시장)
- **Signal filter**: `|direction| ≥ 0.05` (관망 시그널 제외, 명확한 방향 call만)
- **Outcome**: 익일 종가 기준 `actual_return ≠ 0` 인 케이스만
- **Hit**: `sign(direction) == sign(actual_return)` → 적중
- **Window**: 7d / 30d / all-time 동시 산출
- **Per-agent stats**: `n ≥ 5` 샘플 이상만 (소표본 noise 제거)

---

## 🛡️ 무엇을 약속하지 않는가

- ❌ 수익 보장 (자본시장법 §9-4 위반)
- ❌ 1:1 종목 매수·매도 권유 (정보 제공 목적)
- ❌ 100% 정확한 예측 (어떤 시스템도 못 함)

본 ledger는 **신뢰의 증거**일 뿐 투자 권유 자료가 아닙니다.

---

## 🔗 더 보기

- **NAVIGATE 무료 텔레그램**: https://t.me/ai_finance_signal_bot?start=free
- **블로그**: https://blog.naver.com/navigatekai
- **웹사이트**: https://navigate-ai.co.kr (5/21 자본시장법 §101 신고 후 정식 launch)

---

*본 ledger는 정보 제공 목적이며 개별 투자상담이 아닙니다. 투자 판단과 손익은 전적으로 본인 책임입니다.*

*자본시장법 제101조 유사투자자문업 신고 진행 중 (2026-05-21 집체교육 후 금감원 신고 예정).*

*상호: 네비게이트(NAVIGATE) · 사업자등록번호 154-05-03667*
