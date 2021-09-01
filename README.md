# zifter's helm charts

## List of helm charts
* [domain-exporter](charts/domain-exporter/README.md)

## Contributing
### Testing helm charts
Install [ct](https://github.com/helm/chart-testing/releases)

Run linting of all helm charts
```bash
ct lint
```

### Generate values.schema.json
Install special plugin to generate schema
```bash
helm plugin install https://github.com/karuppiah7890/helm-schema-gen.git
```

Run generation in particular chart folder
```bash
helm schema-gen tests/template-all/values-full.yaml > values.schema.json
```
