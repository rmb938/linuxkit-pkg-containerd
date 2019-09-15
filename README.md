# linuxkit-pkg-containerd
LinuxKit Package for ContainerD

## Usage

For full usage examples see https://github.com/rmb938/k8s-on-linuxkit

### Mounts

See `build.yml` for mount information.

`/run/node` and `/var/node` are created in the root namespace and mounted in various ways to store configuration and database files.

```yaml
- name: containerd
  image: docker.pkg.github.com/rmb938/linuxkit-pkg-containerd/containerd:${VERSION}-amd64
  cgroupsPath: podruntime/cri-containerd
```
