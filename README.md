# RMW_Zenoh and LLM Integration

This project aims to combine the high-performance communication infrastructure provided by Zenoh in ROS2 applications with advanced Large Language Model (LLM) integration. The goal is to enable natural language processing and command interpretation capabilities within robotic systems while ensuring efficient and flexible data exchange.

## Table of Contents

- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Contribution](#contribution)
- [License](#license)
- [Contact](#contact)

## Features

- **Zenoh-Based Communication:** Utilizes Zenoh-based RMW (ROS Middleware) for efficient communication in ROS2 applications.
- **LLM Integration:** Connects with large language models (e.g., OpenAI, HuggingFace) to enable natural language processing and interactive command handling.
- **Low Latency:** Ensures real-time data exchange and fast response times.
- **Modular and Flexible Architecture:** Designed to be easily extensible and customizable.

## Requirements

- **Operating System:** Ubuntu (other Linux distributions or Windows via WSL are also supported)
- **ROS2:** Compatible version of ROS2 (e.g., Foxy, Humble)
- **Zenoh:** Zenoh library and associated tools
- **Programming Languages:** C++ and/or Python (depending on the components of the project)
- **LLM API Access:** API keys for your preferred LLM service provider (e.g., OpenAI API key)

## Installation

### 1. Clone the Repository

```bash
git clone https://github.com/your_username/RMW_Zenoh_LLM_Integration.git
cd RMW_Zenoh_LLM_Integration
```

### 2. Install Dependencies

#### ROS2 and Zenoh Dependencies

Ensure that ROS2 and the required Zenoh packages are installed on your system. For example, if you're using ROS2 Foxy on Ubuntu:

```bash
sudo apt update
sudo apt install ros-humble-<package_name>
sudo apt install ros-humble-rmw*
```

For Zenoh, please refer to the official documentation: [Zenoh Installation](https://zenoh.io)

#### Python Dependencies

Install the necessary Python libraries for LLM integration:

```bash
pip install -r requirements.txt
```

### 3. Configuration

Edit the configuration files (e.g., `config.yaml` or `.env`) in the project directory to set your LLM API keys, Zenoh settings, and any other parameters.

## Usage

### ROS2 and Zenoh Integration

To launch your ROS2-based application with Zenoh integration, run:

```bash
ros2 launch rmw_zenoh_integration rmw_zenoh_launch.py
```

### LLM Integration

A sample Python script is provided to interact with the LLM. You can test the LLM integration using the following command:

```bash
python llm_integration.py --prompt "Hello, how can the robot assist you?"
```

This command sends a request to the configured LLM API and prints the response to the console.

## Contribution

Contributions are highly welcome! If you find any bugs, have suggestions, or want to add new features, please follow these steps:

1. Fork the repository.
2. Create a new branch: `git checkout -b feature/your-feature-name`
3. Make your changes and commit them.
4. Push your branch and open a Pull Request.

Feel free to open an issue or contact us directly for any questions or suggestions.

## License

This project is licensed under the [MIT License](LICENSE). See the license file for more details.

## Contact

For any questions, suggestions, or feedback, please reach out via:

- **Email:** [faruk.gmstss@gmail.com](mailto:email@example.com)
- **GitHub:** [ahmet-f-gumustas](https://github.com/your_username)

