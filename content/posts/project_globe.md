---
title: "Project: Toy globe"
date: 2025-06-29T20:50:51-07:00
projects: ['Science', 'Animation', 'Blender']
draft: false 
---

### Goal
Visualize NASA true-color data on a toy globe.

### Data preparation
Topgraphy: [NASA topography data](https://neo.gsfc.nasa.gov/view.php?datasetId=SRTM_RAMP2_TOPO)

NASA blue marble images (360x180px): [NASA blue marble](https://neo.gsfc.nasa.gov/view.php?datasetId=BlueMarbleNG)

The code to create a combined table capturing topography (height) and r, g, b, values per latitude and longitude can be found in the [toy-globe Github repo](https://github.com/JensAdamczak/toy-globe/tree/main).

### Animation
The animation is created in Blender using geometry nodes.

![globe blender](img/project_globe/globe.png)
