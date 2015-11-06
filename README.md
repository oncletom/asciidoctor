# asciidoctor

> Docker image to build asciidoctor project.

**Asciidoctor version** corresponds to the one listed in the `Gemfile`. Currently, the `1.5` branch.

# Build

```bash
make build
```

# Run

```bash
docker run -i --rm \
  -v $(PWD):/documents \
  oncletom/asciidoctor \
  -b html5 \
  -d book \
  -D dist/document.html \
  document.adoc
```
