A virtual reality prototype built in Unity 2022.3 LTS demonstrating basic locomotion, physics-based object manipulation, and input simulation using the XR Interaction Toolkit.

🚀 Features

XR Origin Architecture: Integrated XR Origin (Action-based) rig supporting head tracking and dual controller input.

Teleportation Locomotion: Ground plane configured with Teleportation Area components linked to a central Teleportation Provider.

Physics Object Interaction: Interactive 3D cubes featuring XR Grab Interactable, Rigidbody, and Box Collider components, enabling direct grabbing, moving, and releasing mechanics.

Input Simulation: Configured with the XR Device Simulator and standard Input Action Manager bindings for desktop testing without requiring physical headset hardware.

🛠️ Project Setup & Tech Stack

Unity Version: 2022.3 LTS

XR Plugin Management: OpenXR Framework

Toolkit: XR Interaction Toolkit (XRI)

🎮 How to Run

Open the project in Unity 2022.3 LTS.

Open the main scene located in Assets/Scenes/SampleScene.unity.

Press the Play button in Unity.

Simulator Controls:

Use WASD / Mouse to navigate the virtual camera view.

Hold the right mouse button to manipulate virtual controllers.

Use Teleportation Ray to aim at the ground plane and trigger movement.

Move controller interactors into collision range of the cubes and trigger the Select/Grip action to grab, carry, or throw objects.

📝 Project Summary & Encountered Issues

Project Summary

Successfully set up a functional VR environment using OpenXR and the Unity XR Interaction Toolkit. Built an environment with teleportation zones and interactive physics objects. Verified room-scale locomotion, collision handling, and object grabbing both in editor simulation and standalone build modes.

Problems Encountered & Resolutions

Input System Binding Mismatches: Initial InvalidOperationException errors were encountered due to incorrect action property bindings on controller components. Resolved by updating the Action Reference assignments on the action-based controllers.

Grab Interaction Calibration: Fine-tuning precise object-grabbing mechanics via the ray and direct interactors presented challenges during desktop simulation, as ray alignment and collider triggers required exact positioning to consistently register select actions.

📹 Demonstration Video

The demonstration video showing scene setup, teleportation, controller tracking, and object grabbing is available directly within this repository.
