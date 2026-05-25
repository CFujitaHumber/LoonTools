# LoonTools

LoonTools is a wrapper for various commands
featuring diagnostics.

When run inside the ZED container, `--colcon` now sources ROS in the same shell that runs the build and uses `sudo` only for apt metadata refresh and dependency installation. The build itself runs as the normal container user against the writable mounted workspace.

Usage: LoonTools [options]

Options:
    --doctor        Run the Loon Doctor diagnostics
    -c, --colcon       Run colcon build in the current workspace
    -h, --help      Show help
    -v, --verbose   Enable verbose mode
    --dry-run       Do not execute changes
    --version       print version