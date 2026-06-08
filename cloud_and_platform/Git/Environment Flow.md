# Environment Flow

```text
DEV → PPT (PRETST) → TST → PPR (PREPRD) → PRD
```

| Branch       | Real Meaning              | Priority           |
| ------------ | ------------------------- | ------------------ |
| DEV          | Developer Integration     | Mandatory          |
| PPT / PRETST | Technical Pre-Testing     | Optional or Needed |
| TST          | Formal QA Testing         | Mandatory          |
| PPR / PREPRD | Staging (Production-like) | Optional or Needed |
| PRD          | Production                | Mandatory          |
