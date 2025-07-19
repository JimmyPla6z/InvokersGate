# Invoker’s Gate

A graphical front-end for launching applications using the `RunAsInvoker` compatibility flag.

## Overview

Invoker’s Gate is a lightweight Windows HTA application that acts as a GUI wrapper for launching programs under the `RunAsInvoker` execution context. This allows applications to inherit the parent process's privileges without prompting for UAC elevation—ideal for testing behavior, bypassing elevation prompts, or running tools in constrained environments.

Designed to be simple, portable, and compatible with legacy Windows environments, Invoker’s Gate provides visual feedback on status and supports script integration.

## Features

- GUI-based launcher for `RunAsInvoker` executions
- Supports drag-and-drop and manual path input
- Optional logging and status feedback
- Built with HTA for low overhead and high compatibility
- No external dependencies beyond Windows HTA support

## What is `RunAsInvoker`?

`RunAsInvoker` is a Windows compatibility setting that forces a process to run with the same access token as its parent, bypassing standard UAC elevation. This is especially useful when testing privilege-sensitive code or avoiding elevation prompts in controlled environments.

Invoker’s Gate makes this capability more accessible by wrapping it in a graphical interface.

## Installation

### Option A: Use The Installer
- Go to the [releases page](https://github.com/JimmyPla6z/InvokersGate/releases)
- Click on the WinGUILite-Installer.exe, which will automatically download the installer
- Run the installer.
- Once the installer is completed, launch the app and start bypassing UAC prompts ethically.

### Option B: Clone the Repository
Clone the repository and launch the HTA via using these three commands:

```bash
git clone https://github.com/JimmyPla6z/InvokersGate.git
cd InvokersGate
start RunAsInvoker.hta
