
# Neuropixels trajectory explorer with Sutter Manipulator integrated
Neuropixels trajectory explorer with the Allen CCF mouse atlas 

There is also a Waxholm rat atlas version available, though this is not actively maintained.

The program does not require any specific software. It was written and can be run from MATLAB, but included is a standalone version that does not require MATLAB to run.

**Features:**
  * Plan trajectories to target brain regions with one or more Neuropixels probes
  * Interface with New Scale manipulators to have a live visual of trajectories and recorded areas during an experiment
  * Display brain regions alongside data during recording (in Open Ephys or SpikeGLX)

**For a demo, see [this video](https://www.youtube.com/watch?v=54VHDqzowwY&ab_channel=MatteoCarandini) (part of the [2023 UCL Neuropixels Course](https://www.ucl.ac.uk/neuropixels/training/2023-neuropixels-course))**


**For instructions, see the [Wiki](https://github.com/petersaj/neuropixels_trajectory_explorer/wiki)**

**Updates and issues:**
  * **Regularly pull new code:** try to use up-to-date code whenever possible, there are sometimes critical fixes/updates
  * Major changes are logged on the [Wiki change log page](https://github.com/petersaj/neuropixels_trajectory_explorer/wiki/Major-change-log)
  * Issues/bugs/suggestions: please open a github issue by clicking on the 'Issues' tab above and pressing the green 'New issue' button
  * Planned updates are marked as "future upgrades" on the issues page (https://github.com/petersaj/neuropixels_trajectory_explorer/issues). If you would like to be notified when a planned update is completed, click into the issue page for that update and hit "subscribe" in the lower right-hand corner

![](https://github.com/petersaj/neuropixels_trajectory_explorer/blob/main/wiki/example_trajectory/1.png)

## Sutter Micromanipulator Integration

To utilize the Sutter Micromanipulator with the Neuropixels Trajectory Explorer, follow the steps below for connection and calibration:

### Connecting the Sutter Micromanipulator

1. **Access the Sutter Connection**: From the upper menu of the Neuropixels Trajectory Explorer interface, select `Manipulator` and then `Sutter`.

2. **Select the COM Port**: 
   Identify the COM port to which the Sutter Micromanipulator is connected. This can typically be found in your computer's device settings. Here are some tips to locate the COM port:
   - **Windows**: Navigate to `Device Manager -> Ports (COM & LPT)` and look for a listing that corresponds to the Sutter device.
   - **Mac/Linux**: Open a terminal window and type `ls /dev/tty.*` or `ls /dev/serial/by-id/` and locate the device name linked to the Sutter.

### Calibrating the Sutter Micromanipulator

1. **Manipulator Alignment**: Carefully align the manipulator so the probe makes gentle contact with Bregma.

2. **Zeroing the Manipulator**: After ensuring proper alignment, click on `Zero Manipulator`. This will calibrate the manipulator by setting the current position as the baseline for all subsequent movements within the brain
