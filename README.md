# Container images for toolbx

Container images to use with [toolbx] ([GitHub]).

## Available distributions and usage

- Fedora: See the official images (default in toolbx)

- [Arch Linux]:
  ```
  $ toolbox create --image quay.io/toolbx-images/archlinux-toolbox:latest
  $ toolbox enter archlinux-toolbox-latest
  ```

- [CentOS (Stream)]:
  ```
  $ toolbox create --image quay.io/toolbx-images/centos-toolbox:stream9
  $ toolbox enter centos-toolbox-stream9
  ```

- [Debian]:
  ```
  $ toolbox create --image quay.io/toolbx-images/debian-toolbox:unstable
  $ toolbox enter debian-toolbox-unstable

  $ toolbox create --image quay.io/toolbx-images/debian-toolbox:testing
  $ toolbox enter debian-toolbox-testing

  $ toolbox create --image quay.io/toolbx-images/debian-toolbox:11
  $ toolbox enter debian-toolbox-11

  $ toolbox create --image quay.io/toolbx-images/debian-toolbox:10
  $ toolbox enter debian-toolbox-10
  ```

- [Red Hat Enterprise Linux (Universal Base Image)]. Note: You are free to use
  and redistribute UBI images, provided you adhere to the [Red Hat Universal
  Base Image End User Licensing Agreement][UBI].
  ```
  $ toolbox create --image quay.io/toolbx-images/rhel-toolbox:9.0
  $ toolbox enter rhel-toolbox-9.0

  $ toolbox create --image quay.io/toolbx-images/rhel-toolbox:8.6
  $ toolbox enter rhel-toolbox-8.6

  $ toolbox create --image quay.io/toolbx-images/rhel-toolbox:8.4
  $ toolbox enter rhel-toolbox-8.4

  $ toolbox create --image quay.io/toolbx-images/rhel-toolbox:8.2
  $ toolbox enter rhel-toolbox-8.2
  ```

- [Ubuntu]:
  ```
  $ toolbox create --image quay.io/toolbx-images/ubuntu-toolbox:22.04
  $ toolbox enter ubuntu-toolbox-22.04
  ```

## Hacking on images

As we have limited free GitHub Actions minutes, we do not trigger builds on
PRs, only on merged commits. Please test you image builds locally before
submitting a PR.

[toolbx]: https://containertoolbx.org
[GitHub]: https://github.com/containers/toolbox
[Arch Linux]: https://hub.docker.com/_/archlinux/
[CentOS (Stream)]: https://www.centos.org/centos-stream/
[Debian]: https://hub.docker.com/_/debian
[Red Hat Enterprise Linux (Universal Base Image)]: https://developers.redhat.com/products/rhel/ubi
[UBI]: https://www.redhat.com/licenses/EULA_Red_Hat_Universal_Base_Image_English_20190422.pdf
[Ubuntu]: https://hub.docker.com/_/ubuntu
