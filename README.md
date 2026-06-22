# SDisplay

SDisplay is a lightweight macOS application that visualizes your system's CPU usage through a dynamic animation. The animation speed of the displayed character scales proportionally with your current CPU load.

## Concept and Vision

SDisplay breaks free from being just a macOS menu bar utility. It is designed to be a versatile, free-floating widget that can be placed anywhere on your screen. 

While you can still choose to dock it in the menu bar as a traditional status item, you now have the complete freedom to position it statically anywhere on your desktop. This allows you to integrate the CPU visualization into your personal workspace setup exactly how you want it.

### Key Features

- **Freely Positionable**: Move and place the display at any static location on your desktop screen.
- **Menu Bar Option**: Optionally dock the application in the macOS menu bar for a more traditional experience.
- **Dynamic Hardware Feedback**: The animation speed provides an immediate, intuitive visual representation of your system's CPU load.
- **Lightweight**: Built purely with Swift and AppKit, ensuring minimal system overhead and battery consumption.

## Technical Details

SDisplay leverages low-level Darwin Mach APIs to accurately monitor system CPU ticks in the background. It calculates the delta between system, user, and idle states to determine the precise CPU load, which directly controls the frame interval of the animation.
