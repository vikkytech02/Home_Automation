# Home Automation

This Arduino project allows for the control of an 8-channel relay module using serial communication. It can manage individual relays, execute predefined patterns, and toggle all relays simultaneously. The system is ideal for automation tasks and remote control projects.

---

## Features

- **Individual Relay Control**: Turn each relay ON or OFF using specific commands.
- **Start/Stop All Relays**: Control all relays simultaneously with a single command.
- **Custom Relay Patterns**: Execute predefined patterns for relay operations.
- **Serial Communication**: Commands are sent via Serial Monitor or Bluetooth modules.

---

## Components Used

1. **Arduino Mega**: Microcontroller for managing relay control logic.
2. **8-Channel Relay Module**: Allows control of up to 8 devices or circuits.
3. **Serial Communication Interface**: USB or Bluetooth for sending commands.

---

## Pin Configuration

| Relay        | Arduino Pin |
|--------------|-------------|
| Relay 1      | 2           |
| Relay 2      | 3           |
| Relay 3      | 4           |
| Relay 4      | 5           |
| Relay 5      | 6           |
| Relay 6      | 7           |
| Relay 7      | 8           |
| Relay 8      | 9           |

---

## Commands

| Command | Action                            |
|---------|-----------------------------------|
| A       | Turn Relay 1 OFF                 |
| a       | Turn Relay 1 ON                  |
| B       | Turn Relay 2 OFF                 |
| b       | Turn Relay 2 ON                  |
| C       | Turn Relay 3 OFF                 |
| c       | Turn Relay 3 ON                  |
| D       | Turn Relay 4 OFF                 |
| d       | Turn Relay 4 ON                  |
| E       | Turn Relay 5 OFF                 |
| e       | Turn Relay 5 ON                  |
| F       | Turn Relay 6 OFF                 |
| f       | Turn Relay 6 ON                  |
| G       | Turn Relay 7 OFF                 |
| g       | Turn Relay 7 ON                  |
| H       | Turn Relay 8 OFF                 |
| h       | Turn Relay 8 ON                  |
| Z       | Turn all relays OFF (stop)       |
| z       | Turn all relays ON (start)       |
| v       | Execute custom relay pattern 1   |

---

## How It Works

1. **Serial Commands**: Commands are sent via the Serial Monitor or an external device.
2. **Start/Stop**: Use `z` to turn all relays ON and `Z` to turn them OFF.
3. **Custom Pattern**: Use the `v` command to execute a predefined sequence of relay activations.

---

## Installation and Usage

1. **Wiring**: Connect the relays to the Arduino as per the pin configuration table.
2. **Upload Code**: Upload the code to your Arduino Mega using the Arduino IDE.
3. **Serial Monitor**: Open the Serial Monitor and set the baud rate to `9600`.
4. **Send Commands**: Enter commands to control the relays as per the table above.

---

## Notes

- Relays are active LOW, meaning they are ON when the pin is set to LOW.
- Ensure the relays can handle the voltage and current of the connected devices.
- Add appropriate delay intervals for mechanical relays to avoid rapid switching.

---

## License

This project is open-source and licensed under the [MIT License](LICENSE).

---

## Contributing

Contributions are welcome! Feel free to fork this repository and submit pull requests.

---

## Contact

For questions or feedback, please reach out or raise an issue in the repository.
