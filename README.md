
# 2110363 Hardware Synthesis Lab - Term Project

This project implements a basic computer terminal using an FPGA, supporting USART serial communication and VGA display. The terminal functions as both a receiver and sender for displaying ASCII characters and transmitting data in a  VGA display environment.

This README provides an overview of the project objectives, requirements, and grading criteria for a term project in Hardware Synthesis.

## Project Objectives

- **Design Goal**: Build a functional computer terminal capable of receiving and displaying characters on a VGA screen and sending data over a USART interface.
- **Core Components**: VGA display, USART communication, input switches, and optional PS/2 keyboard input.

## Features and Functionalities
### Core Functionalities
- [ ] **VGA Display**:
  - 320x240 resolution, black-and-white output.
  - Displays ASCII characters (`A-Z`, `a-z`, `0-9`, `\n`).
  - Unsupported characters are displayed as `-`.
  - Each character displays for 1 second.

- [ ] **USART Interface**:
  - Configured as 8n1 with a baud rate of 9600bps.
  - Supports both receiving and sending of 8-bit data.

- [ ] **Switch-Based Input and Sending**:
  - 8 switches for an 8-bit data input.
  - Push button to send data through USART.

- [ ] **Reset Button**:
  - Allows resetting the terminal state.

- [ ] **Optional Keyboard Input**:
  - PS/2 keyboard (optional) to send 8-bit data over serial on keypress.

### Optional (Bonus) Features
- [ ] **Thai character support** for VGA display.
- [ ] **Graphic design enhancements** for VGA output.
- [ ] **Multi-line text display** on VGA.

## Hardware Requirements

- **Basys3 Board**: The project is designed to run on Basys3 FPGA board.

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/tonklaw/2110363-hws-project.git
   ```

2. Load the project files into your FPGA development environment (e.g., Vivado).

3. Build and program the Basys3 with the synthesized design.

4. **Send Data**: Use the 8 switches to input data and press the push button to send over serial.
5. **Receive Data**: Use USART to send ASCII data to the FPGA and view it on the VGA display.

6. (Optional) Connect a PS/2 keyboard for direct data entry and display.

## Project Author

- Tonkla W. (https://github.com/tonklaw)
- Chatdanai P. (https://github.com/PhorDotC)

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
