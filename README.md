Dockerfile that installs both Danger-swift and Swiftlint
To use, just add the following to your actions yaml:

```yaml
    runs-on: ubuntu-latest
    name: "Run Danger"
    steps:
      - uses: actions/checkout@v1
      - name: Danger
        uses: clutter/danger-swift-swiftlint-action@0.2.0
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}

```
