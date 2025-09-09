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

Below is a step-by-step table for the basic Git workflow used in this project.  
Refer to it for branching, merging, and collaborating best practices.

| #  | Action                           | Command / GitHub Action                             | Description                                         | HEAD (local)              | origin (remote/GitHub)    | Which gets updated?    | Optional?                                  |
|----|----------------------------------|-----------------------------------------------------|-----------------------------------------------------|---------------------------|---------------------------|-----------------------|--------------------------------------------|
| 1  | Clone repo                       | git clone <repo-url>                                | Download repo from GitHub                           | main                      | main                      | Both                  | No                                         |
| 2  | Check status                     | git status                                          | See what's changed                                  | current branch            | -                         | -                     | No                                         |
| 3  | Stage changes                    | git add .                                           | Add all changes to staging                          | current branch (staged)   | -                         | HEAD (local)           | No                                         |
| 4  | Commit changes                   | git commit -m "message"                             | Save changes with a message                         | current branch (commit)   | -                         | HEAD (local)           | No                                         |
| 5  | Pull latest                      | git pull origin main                                | Get newest code from GitHub                         | main (updated)            | main                      | Both                  | No                                         |
| 6  | Push changes                     | git push origin main                                | Upload commits to GitHub                            | main                      | main (updated)            | origin (remote)        | No                                         |
| 7  | New feature branch               | git checkout -b feature-branch                      | Create and switch to new branch                     | feature-branch            | -                         | HEAD (local)           | No                                         |
| 8  | Switch branches                  | git checkout main                                   | Switch back to main branch                          | main                      | -                         | HEAD (local)           | No                                         |
| 9  | Push new branch                  | git push origin feature-branch                      | Upload feature branch to GitHub                     | feature-branch            | feature-branch (new)      | origin (remote)        | No                                         |
| 10 | Merge feature into main (local)  | git checkout main; git merge feature-branch          | Copy changes from feature to main (locally)         | main (with merged commit) | -                         | HEAD (local)           | Yes                                        |
| 11 | Push main after merge (local)    | git push origin main                                | Upload merged changes to GitHub main                | main                      | main (updated)            | origin (remote)        | Yes                                        |
| 12 | Create a PR on GitHub (optional) | GitHub UI (“Compare & pull request”)                | Propose merging feature-branch into main            | -                         | PR created (no branch)    | origin (remote)        | Yes (alternative to 10/11)                 |
| 13 | Merge a PR on GitHub (optional)  | GitHub UI (“Merge pull request”)                    | Apply feature-branch changes into origin/main       | -                         | main (updated)            | origin (remote)        | Yes (alternative to 10/11)                 |
