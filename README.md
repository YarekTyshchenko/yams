# Yet Another Modbus Simulator

![YAMS](yams.png)


A simulator for Modbus client/server that supports YAML based configuration and behavior definition, with pure Rust.

YAMS supports Modbus device configuration and behavior definition via YAML files. This means one can predefine how the
simulator works before running the simulator, including:

- the device type: Server/Client
- the protocol type: Modbus TCP/RTU
- communication configurations: IP address, baudrate, etc.
- Modbus configurations: device ID etc.
- Modbus server properties:
    - supported function codes
    - supported registers/coils and their values
- Modbus client behaviors:
    - requests to send to server(s)
    - support repeated request
    - support predefined delay before a request
- Human friendly UI:
    - flexible request organization
    - set and show measurements in its own type: 32-bit float

## Quick Demo:

[DEMO 1](https://asciinema.org/a/451879)

## Todo:

- [x] implement Modbus TCP support
- [x] implement YAML configuration/request support
- [ ] implement Modbus RTU support
- implement function code support below:
  - [ ] Read Coils
  - [ ] Read Discrete Inputs
  - [ ] Read Holding Registers
  - [x] Read Input Registers
  - [ ] Write Single Coil
  - [ ] Write Single Register
  - [ ] Read Exception Status
  - [ ] Diagnostics
  - [ ] Get Comm Event Counter
  - [ ] Get Comm Event Log
  - [ ] Write Multiple Coils
  - [ ] Write Multiple Registers
  - [ ] Report Server ID
  - [ ] Read File Record
  - [ ] Write File Record
  - [ ] Mask Write Register
  - [ ] Read/Write Multiple registers
  - [ ] Read FIFO Queue
  - [ ] Encaptulated Interface Transport
  - [ ] CANopen General Reference Request and Response PDU
  - [ ] Read Device Identification
