# Serial Metamorphic Manipulator ROS2

A modular ROS 2 software framework for the subclass of Serial Metamorphic Manipulators. Here all info for using each repo are presented. This is your start-point for SMMs!!!

## Overview

This project provides a modular **ROS 2 software framework** for the modeling, synthesis, evaluation, and visualization of **Serial Metamorphic Manipulators (SMMs)**.

**This is NOT a ROS package!** It provides info on all ros_pkgs developed for SMMs. The design framework implemented for SMMs is briefly discussed and the role of each ros_pkg is presented!

The framework is designed to support the full pipeline of SMM development, from structure generation to performance analysis, using a combination of screw-theoretic modeling, automated configuration, and ROS-integrated tools.

At its core, the system is built around the `smm_screws` package, which implements the fundamental mathematical and computational infrastructure. This includes:

- screw-theoretic representations of robotic systems  
- analytical kinematics and dynamics formulations  
- a YAML-based robot description loader for automatic structure configuration  
- a robot context abstraction that links structural definitions with computational modules  

On top of this core layer, additional packages extend the framework’s capabilities:

- `smm_synthesis` enables the generation of SMM robot structures based on predefined rules and user-defined YAML parameters  
- `smm_metrics` provides performance evaluation tools for analyzing robot characteristics such as manipulability and workspace properties  
- `smm_viz_tools` offers visualization utilities, primarily through RViz, for inspecting robot configurations and computed metrics  

The framework follows a **generated-data driven workflow**, where robot structures and intermediate results are stored in YAML format. These runtime-generated files are organized in a user-defined `smm_data` directory, which acts as a shared data layer between nodes and packages.

To be updated...

## Repository Structure

The framework is organized as a set of modular ROS 2 repositories, each covering a distinct part of the SMM software stack.

- [`smm_screws`](https://github.com/StravopodisNikos/smm_screws)  
  Core screw-theory package providing robot representations, YAML-based loading utilities, robot context abstractions, and analytical kinematics/dynamics tools.

- [`smm_synthesis`](https://github.com/StravopodisNikos/smm_synthesis)  
  Structure synthesis and robot generation package for creating valid SMM configurations based on predefined rules and user-defined YAML inputs.

- `smm_viz_tools`  
  Visualization package for RViz-based inspection of robot structures, frames, and computed results.  
  *(link to be added)*

- `smm_metrics`  
  Performance evaluation package containing metrics for robot analysis and comparison.  
  *(link to be added)*

## Package Roles

The repositories are designed to work together as a modular framework:

- `smm_screws` provides the core mathematical and computational backbone.
- `smm_synthesis` generates robot structures and runtime model data.
- `smm_metrics` evaluates generated robots using performance measures.
- `smm_viz_tools` visual tools

## Workspace Setup

## Installation and Build

To start using the framework do:

```text
mkdir -p ~/ros2_ws/src/smm_class_pkgs
cd ~/ros2_ws/src/smm_class_pkgs

mkdir ./smm_data

git clone https://github.com/StravopodisNikos/smm_screws.git
git clone https://github.com/StravopodisNikos/smm_synthesis.git
git clone https://github.com/StravopodisNikos/smm_metrics.git
git clone https://github.com/StravopodisNikos/smm_viz_tools.git
```

## Example Workflow

## Current Status

## Roadmap

## Media / Demonstrations

## License

This project is licensed under the BSD 3-Clause License.
