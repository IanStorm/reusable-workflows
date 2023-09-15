# Reusable workflows

Garage project for **private purposes**.
Provides reusable workflows for GitHub Actions.


## How to use in "production"? 👨‍💼 👩‍💼


### Settings

```yaml
# [...]

jobs:
  check-job:
    uses: IanStorm/reusable-workflows/.github/workflows/settings.yml

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
