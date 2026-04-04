# Serial Metamorphic Manipulator ROS2

A modular ROS 2 software framework for the subclass of Serial Metamorphic Manipulators. Here all info for using each repo are presented. This is your start-point for SMMs!!!

## Overview

This project provides a modular **ROS 2 software framework** for the modeling, synthesis, evaluation, and visualization of **Serial Metamorphic Manipulators (SMMs)**.

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

## Package Roles

## Workspace Setup

## Installation and Build

## Example Workflow

## Current Status

## Roadmap

## Media / Demonstrations

## License

This project is licensed under the BSD 3-Clause License.
