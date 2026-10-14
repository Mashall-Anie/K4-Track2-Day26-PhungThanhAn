# K4 · Track 2 · Day 26 — Colosseum Agent Arena

**Nhóm / Team:** PhungThanhAn (làm việc cá nhân · solo)

| Họ và tên | MSSV |
|---|---|
| Phùng Thành An | 2A202603006 |

## Nội dung nộp · Deliverables

- `PhungThanhAn.bundle` — tạo bởi `make submit TEAM=PhungThanhAn` (chứa `agent/`, `deck/`, `eval/`, manifest và sha256 của toàn bộ `kit/`).
- Mã nguồn trong repo: `agent/gateway.py`, `agent/guardrails.py`, `agent/prompt.md`, `deck/deck.json`, `deck/lineup.json`, `eval/prosecute.py`.

## Kết quả kiểm tra tại thời điểm nộp · Checks at submission time

- `make test` — 4608 passed, 7 skipped
- `make validate` — PASS, 0 FAIL (deck 14 thẻ: 10 attack / 4 blank; 5 MCP, 2 gateway, 3 A2A; 9 lớp tấn công khác nhau)
- `python -m eval.prosecute` — precision 1.000 / recall 1.000 trên 40 fixture (baseline 1.000 / 0.059)
- `python spar.py --bot rookie|operator|adversary` — 100–0 / 100–0 / 72–0
- `git status kit/ bots/ fixtures/` — sạch (không sửa file nào trong hash gate)