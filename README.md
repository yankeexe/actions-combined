## 🤜🏼🤛🏼 Combined Actions

Repository containing multiple composite actions.

> This action is part of the following blog:


<a href="https://yankee.dev/cicd-with-github-composite-actions">
<img src="https://i.imgur.com/yOtKXSe.jpg"  width="500" />
</a>

## 🧩 Actions List

### 👋 greetings

```yaml
name: Some Action

on:
  push:
    branches:
      - main

jobs:
  hello-world:
    runs-on: ubuntu-latest
    steps:
      - name: Greet someone
        uses: yankeexe/actions-combined/actions/greetings@main
        with:
          who-to-greet: "everyone"
```

### 🔗 ping

```yaml
name: Some Action

on:
  push:
    branches:
      - main

jobs:
  pinger:
    runs-on: ubuntu-latest
    steps:
      - name: ping
        uses: yankeexe/actions-combined/actions/ping@main
        with:
          url: "github.com"
          count: 10
          interval: 2
```
