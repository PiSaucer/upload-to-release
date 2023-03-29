# Upload to Release GitHub Action - Node 16

A GitHub Action that uploads a file to a new release.

## Getting Started

```yml
jobs:
  build:
    # ...
    steps:
      - uses: PiSaucer/upload-to-release@1.0.2
        with:
          name: my-artifact
          path: build/a.out
          repo-token: ${{ secrets.GITHUB_TOKEN }}
          content-type: text/plain # Optional
```

## Inspiration

This was inspired by:

- https://github.com/actions/javascript-template
- https://github.com/JasonEtco/upload-to-release

