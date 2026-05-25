# LoonE Script

LoonE is a wrapper for containers.

Allows you to build the containers, enter them, move to the work environment, check status of containers, and build with virtual zedx or hardware zedx settings. 

The ZED container is meant to be used as the regular `robo` user. When maintenance is needed inside that container, run `sudo` for package refresh or dependency installation instead of entering the container as root.

The `--help` flag provides a detailed description of the available options and their usage.

## Example Usage

Building zed service with virtual zedx profile:

```bash
loonE -b --virtual zed
```

Building zed service with hardware zedx profile:

```bash
loonE -b --hardware zed
```

building loone service:

```bash
loonE -b loone
```

Starting loone service:

```bash
loonE -s loone
```

entering loone service container:

```bash
loonE -e loone
```

Inside the ZED container, use `sudo apt-get update` and other `sudo`-prefixed maintenance commands when required. Normal RViz and workspace work should stay non-root.