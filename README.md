Publishes a simple create-react-app to GitHub pages using the new/Beta [actions/deploy-pages](https://github.com/actions/deploy-pages) strategy.

Example workflow:

```yaml
name: deploy
on:
  push:
    branches:
      - 'master'
jobs:
  deploy:
    permissions:
      pages: write
      id-token: write
    uses: binki/binki-action-publish-create-react-app-to-pages/.github/workflows/workflow.yml@1
```
