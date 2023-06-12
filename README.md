**#Clone Repo**
- git clone git@github.com:gsfcosta/deploy-gitlab-runner.git

**#ADD Repo Gitlab**
- helm repo add gitlab https://charts.gitlab.io

**#Update Helm repos**
- helm repo update gitlab

**#Install gitlab runner with values**
- helm install --namespace gitlab gitlab-runner -f gitlab-runner/values.yaml gitlab/gitlab-runner --version 0.48.0
