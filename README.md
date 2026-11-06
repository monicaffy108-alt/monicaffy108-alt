# Hi, I build robot learning pipelines on real hardware

Master's applicant (Fall 2027) in robotics — robot learning and dexterous manipulation.

Two repos, one physical hand:

1. **[l20-gesture-sequencer](https://github.com/monicaffy108-alt/l20-gesture-sequencer)** —
   a programmable gesture layer on a 16-DoF LinkerHand L20: YAML gesture presets with smooth
   interpolation, MuJoCo simulation driven by the same URDF the hardware uses, hand
   teleoperation from a single RGB camera (MediaPipe), and tactile closed-loop grasping on
   fingertip pressure sensors.
   Demo: [closed-loop grasp (YouTube Shorts)](https://youtube.com/shorts/fceqbrzrN8s)
2. **[L20-LeRobot-ACT-Grasp](https://github.com/monicaffy108-alt/L20-LeRobot-ACT-Grasp)** —
   vision-conditioned grasping with ACT (Action Chunking with Transformers) via
   [LeRobot](https://github.com/huggingface/lerobot): teleoperated demonstrations recorded as a
   LeRobotDataset, policy trained locally on an RTX 5070, deployed back on the real hand.
   *In progress.*

## Hardware bench

- LinkerHand L20 dexterous hand — 16 active DoF, 5 mimic joints, CAN bus
- XCAN USB CAN adapter
- Intel RealSense D405

## Toolbox

PyTorch · LeRobot / ACT · MuJoCo · CAN bus · Intel RealSense · MediaPipe · Python
