### Intro:

C++ development can be fraught with challenges. From wrangling dependencies to navigating compiler inconsistencies, setting up a new project often feels like navigating a minefield. Here are some of the common pain points:

    Dependency Hell: Traditional C++ package managers (CPM, Conan, vcpkg) often fall short when a required dependency isn't available. This forces you to cobble together solutions from various sources, resulting in complex and fragile CMake configurations.

    Compiler Conundrum: Changing the compiler or standard library version for your project can be a Herculean task, often leading to conflicts with your system's existing C++ environment.

    Inconsistent Development Environments: Ensuring consistent development environments across a team can be a nightmare. Different operating systems, package versions, and compiler flags can lead to frustrating "works on my machine" scenarios.


### Goal:

This project provides a robust and reproducible C++ project template, leveraging the power of Nix to eliminate these headaches and provide a streamlined development experience.
