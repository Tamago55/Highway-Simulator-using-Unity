# Japanese Highway Simulator using Unity

## Demonstration

Please see [the presentation slides](Automotive_Highway_Traffic_Simulator.pdf) or the video (Click it!!)

<a href="https://www.youtube.com/watch?v=Lv8UOpgxc_8" target="_blank" rel="noopener noreferrer"><img src="https://www.youtube.com/watch?v=Lv8UOpgxc_8/hqdefault.jpg" alt="Watch the video" style="max-width:100%;"></a>

## About this program

<img src="https://raw.githubusercontent.com/Tamago55/Highway-Simulator-using-Unity/main/pic/Introduction.png" width="30%" alt="Introduction">

<img src="https://raw.githubusercontent.com/Tamago55/Highway-Simulator-using-Unity/main/pic/Modification.png" width="30%" alt="Modification">

<img src="https://raw.githubusercontent.com/Tamago55/Highway-Simulator-using-Unity/main/pic/work0.png" width="30%" alt="work0">

<img src="https://raw.githubusercontent.com/Tamago55/Highway-Simulator-using-Unity/main/pic/work1.png" width="30%" alt="work1">

<img src="https://raw.githubusercontent.com/Tamago55/Highway-Simulator-using-Unity/main/pic/work2.png" width="30%" alt="work2">


## Folder Structure

- Traffic simulation
  - Examples
    - Addons
    - Materials
    - Meshes
    - Prehabs
    - Scenes
      - `Final.unity` (Select this to start the simulation)
    - Scripts
  - Scripts
    - `VehicleAI.cs` (Modified code file)

To start the simulator, click the "Final" file and press play.

## Development/Research Summary

Most of the development time was spent on using assets to seamlessly connect road segments, allowing for realistic vehicle movement. I adapted an intersection simulator asset for use in a highway setting by refining the code and adjusting various parameters.

The modifications in the `VehicleAI.cs` file focus on overtaking and branching behaviors. By default, vehicle movement was random, leading to a snaking pattern. I altered this behavior to ensure that cars only overtake on the right side when encountering slower traffic ahead. Branching probability was set to 80% for demonstration purposes. These changes, along with the parameter adjustments, ensure vehicles navigate the roads without issues.

## Challenges and Solutions

The main challenge was integrating the intersection simulator asset with the highway system. The solution involved heavy customization of the `VehicleAI.cs` script, particularly in the way cars overtake and branch off the highway. By setting a high branching probability and limiting overtaking to the right side, I achieved a more natural and predictable traffic flow.

## References

- Asset: Unity Traffic Simulation
  (https://github.com/mchrbn/unity-traffic-simulation)

The above-mentioned asset was instrumental in building the simulation, with significant modifications made to the original code to suit our specific needs.


