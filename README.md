# read-file-action

Read file contents.

## Usage

```yaml
steps:
  - name: Read package.json
    id: package
    uses: saurabhrai19/copyfileaction@v1
    with:
      path: ./package.json
  - name: Echo package.json
    run: echo "${{ steps.package.outputs.content }}"
```

## License

MIT
