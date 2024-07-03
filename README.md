# Philosophers

## Introduction

The Philosophers project is an exercise in multithreading and process synchronization using mutexes. It simulates the classic Dining Philosophers Problem to explore threading a process, learning how to create threads, and discovering mutexes to avoid data races.

## Features

- **Multithreading**: Each philosopher is implemented as a separate thread.
- **Mutexes**: Mutual exclusion is used to manage fork access between philosophers to prevent deadlocks.
- **Simulation of Basic Needs**: Philosophers alternate between eating, thinking, and sleeping.
- **Deadlock Prevention**: Design and implementation ensure that no deadlocks occur while philosophers pick up forks.
- **Resource Management**: Forks are treated as resources that are shared between threads (philosophers).

## Getting Started

### Prerequisites

- GCC compiler or another C compiler with support for C11
- POSIX Threads library for threading support

### Installation

1) git clone [repository-url] philosophers
2) cd philosophers
3) make all


## Usage

To run the simulation, you need to provide several parameters:
./philo number_of_philosophers time_to_die time_to_eat time_to_sleep [number_of_times_each_philosopher_must_eat]

- **number_of_philosophers**: The number of philosophers and also the number of forks.
- **time_to_die**: The maximum time (in milliseconds) a philosopher can spend without eating before dying.
- **time_to_eat**: The time (in milliseconds) a philosopher will spend eating.
- **time_to_sleep**: The time (in milliseconds) a philosopher will spend sleeping.
- **number_of_times_each_philosopher_must_eat** (optional): If specified, the simulation will stop if all philosophers eat at least this many times.
