## setup-cordova

[![Continuous Integration](https://github.com/buluma/setup-cordova/workflows/Continuous%20Integration/badge.svg)](https://github.com/buluma/setup-cordova/actions)

Setup your GitHub Actions workflow with Apache Cordova.

## Example

```yaml
- name: Use buluma/setup-cordova
  uses: buluma/setup-cordova@v0.0.3
  with:
    exec: |
      cordova platform add android && \
      cordova build --no-telemetry && \
      cp "$(find . -name '*.apk')" .
```

## Acknowledgement

Initially based on [coturiv/setup-ionic](https://github.com/coturiv/setup-ionic).

## License

SPDX-License-Identifier: [MIT](LICENSE)

## Reference

- [Hello world docker action](https://github.com/actions/hello-world-docker-action)

## See Also

- [Setup Leiningen](https://github.com/oxr463/setup-leiningen)
