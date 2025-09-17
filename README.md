## About This Project

This repository is a beginner-friendly Kubernetes (k8s) tutorial.  
It contains various folders, each demonstrating different k8s concepts, resources, or practical exercises.

Explore the folders below to learn about specific Kubernetes topics:

- [basic-kubectl-commands](https://github.com/pal4lyphe/k8s/tree/main/basic-kubectl-commands) – Essential kubectl commands for beginners
- [configmap-and-secret-volumes](https://github.com/pal4lyphe/k8s/tree/main/configmap-and-secret-volumes) – Using ConfigMaps and Secrets as volumes
- [container-communication-k8s-networking](https://github.com/pal4lyphe/k8s/tree/main/container-communication-k8s-networking) – Pod and container networking basics
- [demo-kubernetes-components](https://github.com/pal4lyphe/k8s/tree/main/demo-kubernetes-components) – Demonstrations of key Kubernetes components
- [github-actions](https://github.com/pal4lyphe/k8s/tree/main/github-actions) – Integrating GitHub Actions with Kubernetes workflows
- [kubernetes-configuration-file-explained](https://github.com/pal4lyphe/k8s/tree/main/kubernetes-configuration-file-explained) – In-depth explanation of configuration files
- [kubernetes-ingress](https://github.com/pal4lyphe/k8s/tree/main/kubernetes-ingress) – Working with Ingress resources
- [kubernetes-volumes](https://github.com/pal4lyphe/k8s/tree/main/kubernetes-volumes) – Persistent and ephemeral volumes
- [linode-kubernetes-engine-demo](https://github.com/pal4lyphe/k8s/tree/main/linode-kubernetes-engine-demo) – Linode Kubernetes Engine demonstration
- [prometheus-exporter](https://github.com/pal4lyphe/k8s/tree/main/prometheus-exporter) – Exporting metrics with Prometheus
- [pull-images-from-private-reporsitory-in-k8s](https://github.com/pal4lyphe/k8s/tree/main/pull-images-from-private-reporsitory-in-k8s) – Pulling images from private repositories
- [setup-prometheus-operator](https://github.com/pal4lyphe/k8s/tree/main/setup-prometheus-operator) – Setting up Prometheus Operator

Feel free to use this project to practice and experiment with Kubernetes!

---

## Git Workflow

<img width="1400" height="788" alt="image" src="https://github.com/user-attachments/assets/7d8c1246-53f7-4e5a-bf3f-ba5696e60ad9" />

# Git Workflow - Step by Step

| Step | What You're Doing | Command | Why This Matters |
|------|------------------|---------|------------------|
| **1** | Get the project | `git clone <repo-url>` | Downloads the project to your computer |
| **2** | Check what's changed | `git status` | See what files are modified/new |
| **3** | Get latest changes | `git pull` | Make sure you have the newest code |
| **4** | Create feature branch | `git checkout -b feature/my-feature` | Work on new features separately from main |
| **5** | Make your changes | *(edit files)* | Do your actual work |
| **6** | Stage changes | `git add .` | Tell Git which changes to save |
| **7** | Save changes locally | `git commit -m "Add new feature"` | Create a snapshot of your changes |
| **8** | Upload to GitHub | `git push origin feature/my-feature` | Share your work with others |
| **9** | Create Pull Request | *(on GitHub website)* | Propose merging your feature branch into the main branch. A Pull Request (PR) allows reviews, discussions, and approvals before integration. If you push directly to main, no PR is created |
| **10** | Merge after approval | *(on GitHub website)* | Your changes become part of the main code |
| **11** | Switch back to main | `git checkout main` | Go back to the main branch |
| **12** | Get merged changes | `git pull` | Update your local main with the new changes |

## Quick Reference Commands

### Daily Workflow
```bash
# Start your day
git pull
git checkout -b feature/new-thing

# Do your work, then:
git add .
git commit -m "Clear description of what you did"
git push origin feature/new-thing
```

### Branch Management
```bash
# See all branches
git branch -a

# Switch branches
git checkout main
git checkout feature/my-feature

# Delete old branch (after merging)
git branch -d feature/old-feature
```

### Check Your Status
```bash
# What's changed?
git status

# What's the difference?
git diff

# Recent commits
git log --oneline -5
```

## Common Scenarios

| Situation | Command | Notes |
|-----------|---------|-------|
| **Forgot to pull first** | `git pull` then resolve conflicts | Always pull before starting work |
| **Wrong commit message** | `git commit --amend -m "New message"` | Only if you haven't pushed yet |
| **Want to undo changes** | `git checkout -- filename` | Removes unsaved changes to a file |
| **Made changes on wrong branch** | `git stash` → switch branch → `git stash pop` | Moves uncommitted changes |
| **Need to update branch** | `git checkout main` → `git pull` → `git checkout feature-branch` → `git merge main` | Keep feature branch updated |
