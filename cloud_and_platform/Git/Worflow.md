# Git Branching & Pull Request Flow

```text
┌─────────────────────┐
│ Local Development   │
└──────────┬──────────┘
           │
           │ git status
           │ git add . 
	       | git add <specificfile.py> <specificfile2.py>
           │ git commit -m "message"
           │
           ▼
┌─────────────────────┐
│ Local Branch        │
│ feature/login       │
│ dev                 │
└──────────┬──────────┘
           │
           │ git push origin feature/login
           │
           ▼
┌─────────────────────┐
│ Remote Repository   │
│ GitHub / GitLab     │
└──────────┬──────────┘
           │
           │ Create Pull Request
           │ source: feature/login
           │ target: main
           │
           ▼
┌─────────────────────┐
│ Pull Request (PR)   │
└──────────┬──────────┘
           │
           ├─────────────────────────┐
           │                         │
           ▼                         ▼
┌──────────────────┐      ┌──────────────────┐
│ Automated Checks │      │ Code Review      │
│                  │      │                  │
│ Unit Tests       │      │ Team Approval    │
│ Linting          │      │ Security Review  │
│ SAST             │      │ Architecture     │
└────────┬─────────┘      └────────┬─────────┘
         │                         │
         └───────────┬─────────────┘
                     │
                     ▼
          ┌─────────────────────┐
          │ PR Approved         │
          └──────────┬──────────┘
                     │
                     │ Merge
                     ▼
          ┌─────────────────────┐
          │ Main / Production   │
          │ Branch              │
          └──────────┬──────────┘
                     │
                     │ GitOps / CI-CD
                     ▼
          ┌─────────────────────┐
          │ Production          │
          │ Environment         │
          └─────────────────────┘
```

---

# Ownership View

```text
┌─────────────────────────────┐
│ Local Development           │ ← Developer
├─────────────────────────────┤
│ Pull Request                │ ← Developer
├─────────────────────────────┤
│ Automated Validation        │ ← CI/CD Platform
├─────────────────────────────┤
│ Code Review                 │ ← Senior / Team Lead
├─────────────────────────────┤
│ Merge to Main               │ ← Repository Policy
├─────────────────────────────┤
│ Deployment                  │ ← DevOps / Platform
├─────────────────────────────┤
│ Production                  │ ← Operations / SRE
└─────────────────────────────┘
```