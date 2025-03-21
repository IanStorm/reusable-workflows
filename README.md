# Reusable workflows

Garage project for **private purposes**.
Provides reusable workflows for GitHub Actions.


## How to use in "production"? 👨‍💼 👩‍💼


### Docker

```yaml
# [...]

jobs:
  docker-job:
    uses: IanStorm/reusable-workflows/.github/workflows/_docker.yml@main
    with:
      dockerhub_username: some user
      platforms: linux/amd64,linux/arm/v7 # 👈 optional
      default_branch: main # 👈 optional
    secrets:
      dockerhub_token: some token

# [...]
```


### Node.js

```yaml
# [...]

jobs:
  node-job:
    uses: IanStorm/reusable-workflows/.github/workflows/_node.yml@main

# [...]
```


### Settings

```yaml
# [...]

jobs:
  check-job:
    uses: IanStorm/reusable-workflows/.github/workflows/_settings.yml@main

# [...]
```


## How to develop? 👨‍💻 👩‍💻

Make sure you have installed *Docker* 🐳 and *Visual Studio Code* ♾️.

1. Clone this repository
2. Open the cloned repo in vscode
2. Install the recommended extensions
2. Start editing the workflows (i.e. YML files) under `.github/workflows/` 🤘
* 🔄️ Keep settings files synced via the vscode task `sync`


## Appendix


### Sources 📙

* [GitHub Docs: Reusing workflows](https://docs.github.com/en/actions/using-workflows/reusing-workflows)
