---
permalink: /code/
title: "Code"
excerpt: "Francesco's code"
layout: single
author_profile: true
last_modified_at: 2021-01-01T14:51:23-04:00
toc: true
---


# YARP

[![YARP homepage](https://img.shields.io/badge/YARP-Yet_Another_Robot_Platform-19c2d8.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABYAAAAWCAYAAADEtGw7AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAAB3RJTUUH4QEDEQMztwAfSwAAAhRJREFUOMvVlD9ME2EYxn931x4crVDbajTRwbQSg8ZuDm6NuombBgcTZxMXY4gLySV2YDFMupKwAtESRhIxEQdcIFEjqK1/SsBaWkr/3ZXenUPTUpprA7Ed/Lbvfb7n+d7vyfN+AgCvV89gSMt0YknGFcKhhEiXlsOuOHbuhDvkVurYk29bua/FsgEQ7JOl8cCpYzVsNV+qPI3/yTdr2HYc9rrkSHROGZ2eUbTkhuJzSvVzPqckaskNZXR6RolE55Sw1yUfumOA+M4uWV0nq+nAQW5W04llsgz09LS0QiQyMcnS4nzHzF1anCcyMenAwotg+Zvxl7dvsmeaDPl9TK0nD2C3BgMEvR6cop2Tlh8Lr60Vwys/M7IoVDeJBFnDsGrY+1xp7/JKYqu2L3/PHz4VBcO0Cob9S00TMub+Ra09toghimsd81gU17CICa0m78WF0/1XB/rkdhrvssXyg8+bu3aT1zJuwV7ZEXL3OtsJJ/WKeaTJA4hu57QvWrnSTvhTQa8cWfj5r3Txn6zu7idkaCVwvUEQ+huCrmGRassWOA6CqyGM6aoWCPXawsdHYD1uYL3l+sU7bYUXPjwD7u73wkNuXJrtqhX/n3DVY1UVOTn4ClG6Vkcqxiap9SFUtWzLVFUZX2AZp3y+Xitrs6Tj91FVs5oKh/ss27+Hm6gBRM8IMGX/Vs8IO6lQU/UeDvcY8OMv7HG7CnjlFeQAAAAASUVORK5CYII=)](http://www.yarp.it/)
[![Latest release](https://img.shields.io/github/release/robotology/yarp.svg)](https://github.com/robotology/yarp/releases)
[![Release date](https://img.shields.io/github/release-date/robotology/yarp.svg)](https://github.com/robotology/yarp/releases)

[YARP](https://github.com/robotology/yarp) is a library and toolkit for communication and device interfaces,
used on everything from humanoids to embedded devices.


#  iDynTree
[![License: LGPL v3](https://img.shields.io/badge/License-LGPL%20v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0) [![License: LGPL v2](https://img.shields.io/badge/License-LGPL%20v2-blue.svg)](https://www.gnu.org/licenses/lgpl-2.1)  [![ZenHub](https://img.shields.io/badge/Shipping_faster_with-ZenHub-435198.svg)](https://zenhub.com)

[iDynTree](https://github.com/robotology/idyntree) is a library of robots dynamics algorithms for control, estimation and simulation.

iDynTree is specifically designed for free-floating robots, but it is possible to use it also  with fixed-base robots.

iDynTree is written in C++ language, but thanks to [SWIG](http://www.swig.org/) it is possible to use the iDynTree algorithms in several other languages. Support and documentation is provided in particular for C++, Matlab, Python and Lua.

# whole-body-controllers

The codebase [whole-body-controllers](https://github.com/robotology/whole-body-controllers) contains `Simulink-based whole-body controllers` developed to control the [iCub](http://www.icub.org/) humanoid robot. It can be imagined as a **starting point** and a **support** repository for a user that intends to develop a new Simulink controller (not necessarily for the iCub robot) in within the framework of the [robotology](https://github.com/robotology) organisation. It is worth noting that:

- The controllers stored in this repository are an **overview** of the possibile control frameworks that can be implemented using the `robotology` software infrastructure. Also, the repository contains a [library](library/README.md) of configuration and utility Matlab functions to design simulations with [Gazebo](http://gazebosim.org/) simulator and on the real robot iCub. 

- The robot dynamics and kinematics is computed run-time by means of [WBToolbox](https://github.com/robotology/wb-toolbox), a Simulink library that wraps [iDyntree](https://github.com/robotology/idyntree). For more information on iDyntree library, see also this [README](https://github.com/robotology/idyntree/blob/master/README.md). 

- The Simulink models implement different control strategies both for fixed-base and for floating-base robots. They space from `momentum-based` torque control to `inverse-kinematics-based` position control. Have a look at the [controllers](controllers/README.md) folder for more details.

#  gazebo-yarp-plugins
[![Build Status](https://travis-ci.org/robotology/gazebo-yarp-plugins.svg?branch=master)](https://travis-ci.org/robotology/gazebo-yarp-plugins)

The [gazebo-yarp-plugins](https://github.com/robotology/gazebo-yarp-plugins) are a set of [Gazebo plugins](http://gazebosim.org/) that expose [YARP interfaces](http://yarp.it/)
for robot simulated in Gazebo. The main design objective for the gazebo-yarp-plugins
is to provide the exact same interfaces that can be found in real world YARP-powered
robot in the Gazebo simulation, to ensure that YARP-based software can run with no modifications
both in simulation and on the real robots.
