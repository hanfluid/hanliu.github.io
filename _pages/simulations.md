---
layout: page
title: Simulations
permalink: /simulations/
description: In-house CFD simulations of multiphase turbulent flows.
nav: true
nav_order: 2
---

All simulations on this page were computed with solvers I wrote from scratch.

---

### Ventilated Cavity Flow

Gas injection into an underwater cavity creates complex recirculating flow structures. This DNS captures the cavity dynamics, wake instability, and gas-liquid interaction at low Reynolds number.

{% include video.liquid path="https://www.youtube.com/embed/VJelVY1T58g" class="img-fluid rounded z-depth-1" width="100%" height="400" %}

---

### COVID-19 Airborne Transmission

How did air conditioning spread the virus across a restaurant? This simulation traces respiratory aerosol transport driven by AC airflow, reproducing a real outbreak documented in Guangzhou.

{% include video.liquid path="https://www.youtube.com/embed/NJTRVlPevx4" class="img-fluid rounded z-depth-1" width="100%" height="400" %}

---

### Oil Dispersion Under Breaking Waves

A plunging breaker hits an oil slick. The three-phase solver (air, water, oil) tracks bubble entrainment, droplet breakup, and oil fragmentation simultaneously using a coupled level set method.

{% include video.liquid path="https://www.youtube.com/embed/AhPMyL2Dgl4" class="img-fluid rounded z-depth-1" width="100%" height="400" %}

---

### Turbulent Canopy Flow

Flexible underwater vegetation bends and sways under turbulent flow. This fluid-structure interaction simulation couples the Navier-Stokes equations with structural dynamics to capture the two-way coupling between flow and canopy.

{% include video.liquid path="https://www.youtube.com/embed/256nWAEoTh0" class="img-fluid rounded z-depth-1" width="100%" height="400" %}

---

### 3D Wave Breaking

A three-dimensional plunging breaker captured by DNS. The simulation resolves the full air-water interface evolution, including jet impact, splash-up, bubble entrainment, and spray generation.

{% include video.liquid path="https://www.youtube.com/embed/2ZWy9-J1kdI" class="img-fluid rounded z-depth-1" width="100%" height="400" %}
