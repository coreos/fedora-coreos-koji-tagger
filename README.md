# fedora-coreos-koji-tagger

Source code that monitors a git repo and tags packages over into
appropriate koji tags to be consumed by Fedora CoreOS build processes.

# Rough notes for deployment

Create a new project and build the container.

```
oc new-project fedora-coreos-koji-tagger
oc new-build --strategy=docker https://github.com/coreos/fedora-coreos-koji-tagger --to fedora-coreos-koji-tagger-img
```

Use kedge to get up and running in openshift:

```
kedge apply -f kedge.yaml
```
