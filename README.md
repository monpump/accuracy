# NAVIGATE Lab — Public Accuracy Ledger

**한국어 스마트머니 + AI 비전 인텔리전스의 시그널 정확도 공개 기록**

매일 KST 07:26 (월~토) 운영 PC 의 예약 작업(`write_accuracy_snapshot.py`)이 `signal_log.parquet` 원본 데이터를 재계산하여 [`ACCURACY.md`](./ACCURACY.md)에 prepend합니다.

모든 갱신은 git 이력에 시각과 변경 내용이 남습니다. 지우거나 고친 흔적도 이력에 남습니다 — 그것이 이 기록의 근거입니다.

---

## 📊 검증 방법

1. [`ACCURACY.md`](./ACCURACY.md) 클릭 → 매일 추가되는 entry 확인
2. **git history** 클릭 → 모든 commit 시간 + diff 확인 가능
3. **commit author** = 운영자 계정 (예약 작업이 올림 — 손으로 올린 것과 구분되지 않으므로 이력 전체를 보시면 됩니다)

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

- ❌ 수익 보장 · 손실 보전 (법으로 금지된 약속)
- ❌ 1:1 종목 매수·매도 권유 (정보 제공 목적)
- ❌ 100% 정확한 예측 (어떤 시스템도 못 함)

본 ledger는 **신뢰의 증거**일 뿐 투자 권유 자료가 아닙니다.

---

## 🔗 더 보기

- **블로그**: https://blog.naver.com/navigatekai
- **웹사이트**: https://navigate-ai.co.kr

---

*본 ledger는 정보 제공 목적이며 개별 투자상담이 아닙니다. 투자 판단과 손익은 전적으로 본인 책임입니다.*

*상호: 네비게이트(NAVIGATE) · 사업자등록번호 154-05-03667*
