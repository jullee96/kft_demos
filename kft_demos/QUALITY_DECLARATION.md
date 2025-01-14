This document is a declaration of software quality for the `kft_demos` package, based on the guidelines in [REP-2004](https://www.ros.org/reps/rep-2004.html).

# `kft_demos` Quality Declaration

The package `kft_demos` claims to be in the **Quality Level 4** category.
The main rationale for this claim its its status as a collection of demonstration launch files.

Below are the detailed rationales, notes, and caveats for this claim, organized by each requirement listed in the [Package Requirements for Quality Level 3 in REP-2004](https://www.ros.org/reps/rep-2004.html).

## Version Policy [1]

### Version Scheme [1.i]

`kft_demos` uses `semver` according to the recommendation for ROS Core packages in the [ROS 2 Developer Guide](https://index.ros.org/doc/ros2/Contributing/Developer-Guide/#versioning).

### Version Stability [1.ii]

`kft_demos` is at a stable version, i.e. `>= 1.0.0`.
The current version can be found in its [package.xml](package.xml), and its change history can be found in its [CHANGELOG](CHANGELOG.rst).

### Public API Declaration [1.iii]

`kft_demos` does not have a public API.

### API Stability Policy [1.iv]

`kft_demos` does not have a public API.

### ABI Stability Policy [1.v]

`kft_demos` does not have a public API.

### API and ABI Stability Within a Released ROS Distribution [1.vi]

`kft_demos` does not have a public API.

## Change Control Process [2]

`kft_demos` follows the recommended guidelines for ROS Core packages in the [ROS 2 Developer Guide](https://index.ros.org/doc/ros2/Contributing/Developer-Guide/#package-requirements).

### Change Requests [2.i]

`kft_demos` requires that all changes occur through a pull request.

### Contributor Origin [2.ii]

`kft_demos` uses DCO as its confirmation of contributor origin policy. More information can be found in [CONTRIBUTING](../CONTRIBUTING.md).

### Peer Review Policy [2.iii]

All pull requests must have at least 1 peer review.

### Continuous Integration [2.iv]

All pull requests must pass CI on all platforms supported by RMF.
The CI checks only that the package builds.
The most recent CI results can be seen on [the workflow page](https://github.com/open-rmf/kft_demos/actions).

### Documentation Policy [2.v]

All pull requests must resolve related documentation changes before merging.

## Documentation [3]

### Feature Documentation [3.i]

`kft_demos` is documented in the [parent repository's README.md file](../README.md).

### Public API Documentation [3.ii]

`kft_demos` does not have a public API.

### License [3.iii]

The license for `kft_demos` is Apache 2.0, the type is declared in the [package.xml](package.xml) manifest file, and a full copy of the license is in the repository level [LICENSE](../LICENSE) file.

There are no source files that are currently copyrighted in this package so files are not checked for abbreviated license statements.

### Copyright Statement [3.iv]

There are no copyrighted source files in this package.

### Quality declaration document [3.v]

This quality declaration is linked in the [README file](README.md).

This quality declaration has not been externally peer-reviewed and is not registered on any Level 3 lists.

## Testing [4]

### Feature Testing [4.i]

`kft_demos` is a package providing strictly launch files and therefore does not require associated tests.

### Public API Testing [4.ii]

`kft_demos` is a package providing strictly launch files and therefore does not require associated tests.

### Coverage [4.iii]

`kft_demos` is a package providing strictly launch files and therefore does not require associated tests.

### Performance [4.iv]

`kft_demos` is a package providing strictly launch files and therefore does not require associated tests.

### Linters and Static Analysis [4.v]

`kft_demos` does not use the [standard linters and static analysis tools](https://index.ros.org/doc/ros2/Contributing/Developer-Guide/#linters).

## Dependencies [5]

### Direct Runtime ROS Dependencies [5.i]

`kft_demos` has the following runtime ROS dependencies.

#### kft_demos_maps

`kft_demos_maps` is at [**Quality Level 4**](../kft_demos_maps/QUALITY_DECLARATION.md).

#### rmf_traffic_ros2

`rmf_traffic_ros2` is at [**Quality Level 4**](https://github.com/open-rmf/rmf_ros2/blob/main/rmf_traffic_ros2/QUALITY_DECLARATION.md).

#### rmf_fleet_adapter

`rmf_fleet_adapter` is at [**Quality Level 4**](https://github.com/open-rmf/rmf_ros2/blob/main/rmf_fleet_adapter/QUALITY_DECLARATION.md).

#### building_map_tools

`building_map_tools` is at [**Quality Level 4**](https://github.com/open-rmf/rmf_traffic_editor/blob/main/rmf_building_map_tools/QUALITY_DECLARATION.md).

#### rmf_visualization

`rmf_visualization` is at [**Quality Level 4**](https://github.com/open-rmf/rmf_visualization/blob/main/rmf_visualization/QUALITY_DECLARATION.md).

#### kft_demos_assets

`kft_demos_assets` is at [**Quality Level 4**](../kft_demos_assets/QUALITY_DECLARATION.md).

#### kft_demos_tasks

`kft_demos_tasks` is at [**Quality Level 4**](../kft_demos_tasks/QUALITY_DECLARATION.md).

#### rviz2

`rviz2` does not declare a Quality Level.
It is assumed tobe at **Quality Level 4** based on its widespread use.

#### launch_xml

`launch_xml` does not declare a Quality Level.
It is assumed tobe at **Quality Level 4** based on its widespread use.

### Optional Direct Runtime ROS Dependencies [5.ii]

`kft_demos` does not have any optional direct runtime ROS dependencies.

### Direct Runtime non-ROS Dependency [5.iii]

`kft_demos` does not have any runtime non-ROS dependencies.

## Platform Support [6]

As a pure message and service definitions package, `kft_demos` supports all of the tier 1 platforms as described in [REP-2000](https://www.ros.org/reps/rep-2000.html#support-tiers), but does not currently test each change against all of them.

## Security [7]

### Vulnerability Disclosure Policy [7.i]

This package conforms to the Vulnerability Disclosure Policy in [REP-2006](https://www.ros.org/reps/rep-2006.html).
