# ✅ Getting Started Checklist

## 1. Local environment
- [ ] Git installed and configured (`git config --global user.name` / `user.email`)
- [ ] Latest stable **Go** installed (`go version`)
- [ ] VS Code + **Go extension (gopls)**
- [ ] GitHub **2FA** enabled (required to submit PRs)
- [ ] SSH key or token set up for pushing to GitHub
- [ ] `make` available (optional; can run `go build` / `go test ./...` directly on Windows)
- [ ] Local Kubernetes cluster for testing (`kind` or `minikube`)

## 2. Learn the target project (stern)
- [ ] Install it: `go install github.com/stern/stern@latest`
- [ ] Run it against a test cluster; tail some logs
- [ ] Read `README.md` fully
- [ ] Read `CONTRIBUTING.md` (only ~21 lines) — twice
- [ ] Read the last ~5 merged PRs to learn accepted style
- [ ] Read `stern/stern.go` and `stern/tail.go`

## 3. Fork & build
- [ ] Fork the repo on GitHub
- [ ] `git clone` your fork
- [ ] Add upstream remote: `git remote add upstream https://github.com/stern/stern.git`
- [ ] Build: `go build -o dist/stern .`
- [ ] Test: `go test ./...` (green?)

## 4. First contribution (docs / tiny fix)
- [ ] Find a small target (typo, unclear doc, missing template-func doc, small `help wanted` issue)
- [ ] Open an issue OR comment on an existing one saying you'll take it
- [ ] Wait for a maintainer 👍 before coding
- [ ] Branch: `git switch -c <issue#>-short-name`
- [ ] Make the change; run tests/lint
- [ ] Push to your fork; open PR referencing the issue
- [ ] Write a clear PR description: what it does + how to validate
- [ ] Respond to review feedback; push follow-up commits
- [ ] 🎉 Merged!

## Etiquette reminders
- One focused change per PR. Keep it small.
- Be patient — reviews can take days (volunteers, timezones).
- Don't spam-ping maintainers. Wait several days.
- Review comments are about the code, not you.
