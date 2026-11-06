# SAM – Search and Assist Machine
**Desktop Control & Monitoring System for the Unitree Go2**

SAM (Search and Assist Machine) is a Windows desktop application developed by **Vraith** to control, monitor and interact with the Unitree Go2 robot dog.



## Features
- **Robot Control** – Operate the Go2 using keyboard or gamepad controls.
- **Connection Management** – Connect to compatible Go2 robots over a local network.
- **Monitoring Dashboard** – View available robot information and system status.
- **LiDAR Mapping** – Support for mapping and visualisation features under development.
- **Emergency Stop** – Send a stop command using the spacebar.
- **Windows Application** – Desktop interface built using Electron.
- **Ongoing Development** – Regular improvements to stability, functionality and usability.

> **Note:** SAM is currently under development. Some features may be incomplete or require additional testing with physical hardware.



## Installation

### Windows 10 / 11
1. Visit the [Releases](../../releases) page.
2. Download the latest `SAM-Setup-1.0.0.exe` or newer installer.
3. Run the installer.
4. Follow the installation instructions.
5. Launch **SAM** from your desktop or Start menu.

### System Requirements
| Requirement | Details |
|---|---|
| Operating System | Windows 10 / 11 (64-bit) |
| Robot | Unitree Go2 |
| Connection | Ethernet or supported Wi-Fi |
| Controller | Keyboard or compatible gamepad |

SAM can be opened without a connected robot, but live robot functions require compatible hardware.



## Connecting to Your Robot
### 1. Prepare the Go2
Turn on your Unitree Go2 and wait for it to finish booting.
Ensure the robot is in a safe area with enough space for movement.

### 2. Connect Your Computer
Connect your computer to the robot's supported network using Ethernet or Wi-Fi.
For setups using the `192.168.123.x` network, the following configuration may be used:

| Setting | Value |
|---|---|
| IP Address | `192.168.123.222` |
| Subnet Mask | `255.255.255.0` |
| Default Gateway | `192.168.123.1` |
| Example Robot IP | `192.168.123.161` |

> Confirm these settings match your robot's network configuration before applying them.

### 3. Test Your Connection
Open Command Prompt and run:

```powershell
ping 192.168.123.161
```
If the robot responds, your computer can reach that address.
A successful ping does not guarantee that the robot control connection is available.

### 4. Connect Through SAM
1. Open SAM.
2. Close any conflicting robot control sessions.
3. Click **Connect**.
4. Check the connection status.
5. Verify the connection before attempting movement.



## Controls
### Keyboard
| Key | Action |
|---|---|
| W | Move Forward |
| S | Move Backward |
| A | Turn Left |
| D | Turn Right |
| Q | Sidestep Left |
| E | Sidestep Right |
| Spacebar | Send Emergency Stop Command |

### Gamepad
| Input | Action |
|---|---|
| Left Stick | Movement |
| Right Stick | Turning |

> **Safety:** Software stop commands are not a replacement for physical emergency controls or manufacturer safety procedures.



## Compatibility
SAM is designed primarily for the **Unitree Go2**.
Currently supported target platform:
- Unitree Go2
The Go2 Air and Go2 Pro consumer models are not currently supported.
Compatibility with other Unitree robots and firmware versions has not been verified.


## Development Status
**Status: Active Development**

SAM is an ongoing project, with improvements focused on:

- Robot connection reliability
- Movement and control functionality
- LiDAR mapping and visualisation
- Monitoring and system diagnostics
- Application stability and performance
- User interface improvements
- Hardware testing and bug fixes

Features may change as development progresses.



## Safety Information

SAM controls physical robotic hardware.

Always:

- Operate the robot in a safe environment.
- Keep people and obstacles clear of the robot.
- Follow official Unitree safety instructions.
- Supervise the robot during operation.
- Use the software only with authorised hardware.

## Disclaimer
SAM is an independent project and is not affiliated with, sponsored by Unitree Robotics.
Unitree and Go2 are trademarks of their respective owners.
The software is provided for development, educational and experimental purposes.



**SAM – Search and Assist Machine**
