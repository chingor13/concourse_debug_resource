# Concourse Debug Resource

This is a stub resource that can be used as a no-op that also outputs the inputs of that step.

## Usage

In your `pipeline.yml`:

```
resource_types:
- name: debug-resource
  type: docker-image
  source:
    repository: chingor13/concourse_debug_resource

resources:
- name: some-step
  type: debug-resource
  source:
    foo: bar
```
