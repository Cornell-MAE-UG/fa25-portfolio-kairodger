---
layout: project
title: MAE 4272 Blade Design Project
description: Design, CAD, and Testing
technologies: [Autodesk Fusion 360, MATLAB, Microsoft Office]
image: assets/images/TestingAction.jpg
---

### Project Overview

For this project, our objective was to design and test a wind turbine blade optimized for power extraction while remaining within structural and experimental constraints. The blade was designed to operate in Cornell's Big Blue Wind Tunnel, with constraints on blade length (<6 inches), rotational speed (<2000 RPM), chord length (<2 inches), and wind tunnel flow velocity. We have designed a blade that is expected to be optimal at a wind speed of 7.4 Hz (4.8 m/s). We tested whether the blade holds up structurally at this speed and whether the power output matches our optimization.

<div class="image-row">
  <img src="{{ '/assets/images/bladeCAD.jpg' | relative_url }}" alt="Final CAD">
</div>

### Design Process

For our design process, we started off by using a Weibull distribution to model expected operating conditions and identify an optimal wind speed, which was calculated to be approximately 4.8 m/s. Using this condition, we selected the NACA 4412 airfoil based on good lift-to-drag characteristics at a low Reynolds number that we calculated. From this data, we determined an optimal angle of attack, from which we derived the pitch distribution. We then iterated chord taper ratios under geometric constraints to maximize our predicted power output, which came out to be 0.08 W with a taper ratio of 0.142. Lastly, we ran structural calculations, which showed that there was excessive bending stress at the tip of the initial blade length, so we shortened it from 6 to 4.5 in to bring maximum stress below the material's flexural strength. Using all of these parameters, we made a CAD of the blade.

<div class="image-row">
  <img src="{{ '/assets/images/TwistDist.jpg' | relative_url }}" alt="Twist distribution">
  <img src="{{ '/assets/images/BendingStress.jpg' | relative_url }}" alt="Bending stress">
</div>

### Testing and Results

To test our blade design, the blades were resin printed, assembled, and put into the wind tunnel at multiple flow speeds while gradually increasing the brake torque. From this, we recorded the RPM and power output and generated power curves. The blades reached a maximum power output of approximately 0.17 W at a flow speed of 9 Hz, which exceeded/outperformed our initial calculations of both predicted power output and optimal wind speed. This is most likely because our initial RPM wasn’t chosen at a peak since our initial power curve calculations showed us a graph that increased past 2000 RPM, which exceeds structural limitations. When testing, we also did not see any excess vibrations or structural issues.

<div style="text-align: center;">
<img src="{{ '/assets/images/PowerCurves.jpg' | relative_url }}" width="75%" height="75%">
</div>

### My Contribution

For this project, I contributed to most aspects of the design, notably the initial calculations for optimal wind speed, power output, maximum stress, and pitch distribution. I also helped out with the CAD of the design and data analysis. The team dynamic was very even, so everyone contributed equal amounts.
