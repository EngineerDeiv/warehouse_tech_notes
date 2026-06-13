

```text
DEV → PPT (PRETST) → TST → PPR (PREPRD) → PRD
```

| Branch       | Real Meaning              | Priority           | Purpose                                    |
| ------------ | ------------------------- | ------------------ | ------------------------------------------ |
| DEV          | Developer Integration     | Mandatory          | Develop and integrate new features         |
| PPT / PRETST | Technical Pre-Testing     | Optional or Needed | Validate deployments and technical changes |
| TST          | Formal QA Testing         | Mandatory          | Execute functional and regression testing  |
| PPR / PREPRD | Staging (Production-like) | Optional or Needed | Validate releases before production        |
| PRD          | Production                | Mandatory          | Serve live traffic and business operations |
