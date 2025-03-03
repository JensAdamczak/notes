---
title: "Project: Biomes of the world"
date: 2025-02-15T20:33:30-08:00
projects: ['Science', 'Animation', 'Blender']
draft: false 
---

### Purpose 
A [biome](https://en.wikipedia.org/wiki/Biome) is a distinct geographical region with specific climate, vegetation, and animal life. It consists of a biological community that has formed in response to its physical environment and regional climate.

This project describes the creation of an animation of the distribution of biomes per latitute created in Blender.

### Data preparation
Biome description: [NASA earth observatory](https://earthobservatory.nasa.gov/biome)\
Vegetation index data: [NASA NDVI](https://neo.gsfc.nasa.gov/view.php?datasetId=MOD_NDVI_M)\
Average land temperature: [NASA LSTD](https://neo.gsfc.nasa.gov/view.php?datasetId=MOD_LSTD_CLIM_M)

The code to create the distribution of biomes per latitude can be found in the [biomes-world Github repo](https://github.com/JensAdamczak/biomes-world/tree/main).

![biomes map](img/project_biome/figure_biomes_map.png)

![biomes per lat bin](img/project_biome/figure_biomes_per_lat_bin.png)

### Animation
The animation is created in Blender using geometry nodes. Each biome is represented by a characteristic object/plant. In the animation the objects are placed together on a platform that changes for each latitude bin according to the relative distribution of biomes per latitude in the prepared data.

![biomes overview](img/project_biome/timeline_1_01_00_17_03.png)

![biome render](img/project_biome/biome_render_430.png)

