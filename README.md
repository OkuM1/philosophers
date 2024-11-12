
# Philosophers

Welcome to **Philosophers**! This project is part of the 42 curriculum and is designed to simulate the classic "Dining Philosophers" problem using multithreading in C. The project aims to build proficiency in managing concurrent processes and handling thread synchronization in C. This README outlines the project details, functionality, and achievements.

---

## Table of Contents

- [About the Project](#about-the-project)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Achievements](#achievements)
- [License](#license)

---

## About the Project

The **Philosophers** project simulates the well-known "Dining Philosophers" problem, where philosophers sit at a table and alternate between eating, thinking, and sleeping. Each philosopher needs two forks to eat, which introduces a challenge in synchronization and avoiding deadlocks. The project emphasizes the importance of thread synchronization and resource management.

### Project Objectives
- Implement a multithreaded program that prevents data races and deadlocks.
- Use mutexes to control access to shared resources (forks).
- Enhance understanding of concurrency and resource allocation.

---

## Features

1. **Philosopher Simulation**  
   - Each philosopher alternates between thinking, eating, and sleeping states.
   - Philosophers pick up forks in a specific order to avoid deadlock and starvation.

2. **Thread Synchronization**  
   - Implements mutexes to ensure safe access to shared resources and prevent race conditions.
   - Avoids deadlock through specific fork-picking strategies based on philosopher index.

3. **Customizable Parameters**  
   - Allows customization of the number of philosophers, time to eat, think, and sleep, and maximum simulation duration.

4. **Real-Time Status Updates**  
   - Provides detailed logging of each philosopher’s actions with timestamps.

---

## Installation

To compile the project, clone the repository and use `make`:

```bash
git clone https://github.com/yourusername/philosophers.git
cd philosophers
make
```

This will generate an executable file, `philosophers`, in the project directory.

---

## Usage

To start the simulation, use the following command:

```bash
./philosophers [number_of_philosophers] [time_to_die] [time_to_eat] [time_to_sleep] [optional: number_of_times_each_philosopher_must_eat]
```

Example usage:

```bash
./philosophers 5 800 200 200
```

This command starts a simulation with 5 philosophers where each has 800 ms before dying without food, 200 ms to eat, and 200 ms to sleep.

---

## Achievements

The **Philosophers** project involved overcoming several complex synchronization and concurrency challenges. Here are the main achievements:

- **Deadlock Avoidance**: Implemented custom fork-picking strategies, especially for the philosopher at index 0, ensuring all philosophers can eat without deadlocking or starving.
- **Data Race Prevention**: Used mutexes to protect shared resources and prevent data races, achieving safe multithreading.
- **Dynamic Control over Simulation**: Allowed customizable simulation parameters to accommodate different scenarios, improving flexibility and usability.
- **Real-Time Logging**: Implemented timestamped logs to monitor philosopher activities accurately, aiding in debugging and performance evaluation.
- **Enhanced Concurrency Skills**: Developed advanced understanding of concurrency in C, mastering thread management and resource allocation.

---

## License

This project is licensed under the MIT License. See `LICENSE` for details.

---

Thank you for reviewing **Philosophers**! This project was a valuable experience in mastering thread synchronization and concurrent programming techniques. Feedback and contributions are welcome—please fork the repository and submit pull requests for improvements.

---
