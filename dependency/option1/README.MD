# Just example
## add dependencies
if you want to add dependecies in helm, you can write this in you Chart.yaml

```yaml
dependencies:
- name: database
  condition: enabled.true
  version: 0.1.0
  repository: file://../database
```
and then you can execute the command bellow

```bash
helm dependency update
helm template
```
