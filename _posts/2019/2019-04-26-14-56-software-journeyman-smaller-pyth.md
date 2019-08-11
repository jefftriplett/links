---
categories:
- docker
- multi-stage
- builds
- python
- optimisation
- multistage
external_url: https://softwarejourneyman.com/docker-python-install-wheels.html
shared: true
slug: software-journeyman-smaller-pyth
time: 2019-04-26 14:56:29
title: Software Journeyman – Smaller Python Docker Containers With Multi-Stage Builds
  and Python Wheels
toread: false
---

> If your Docker Python build requires system dependencies that are NOT required at runtime, structure your build as follows: Use a multi-stage build Stage 1 installs system dependencies and uses them to build local wheels Stage 2 begins from the same base as Stage 1, copies wheels from Stage 1, and installs the wheels The rest of your build will be based on Stage 2 If you follow these steps, you'll end up with the smallest-possible Python Docker container with all your Python dependencies intact.