# Netpractice

## What is Netpractice?

Netpractice is a project designed to help students at 42 school learn and practice fundamental networking concepts. The project consists of a series of levels, each presenting a network topology puzzle. The goal is to correctly configure IP addresses, netmasks, and gateways for various devices within the network to ensure connectivity.

The project provides a graphical interface where you can see the network topology, and you need to fill in the correct network configuration for each machine.

## Levels

The project is divided into 10 levels of increasing difficulty:

*   `level1.json`
*   `level2.json`
*   `level3.json`
*   `level4.json`
*   `level5.json`
*   `level6.json`
*   `level7.json`
*   `level8.json`
*   `level9.json`
*   `level10.json`

Each JSON file represents a level and contains the network topology for that level.

## How to use it

You typically use a visualizer tool provided by the school to load and interact with the levels. You will need to input the correct IP addresses and netmasks for the machines and the correct gateway routes to make the network functional.

## Evaluation

The evaluation is done automatically by a program. The evaluator will pick 3 levels at random from the 10 available levels. You will have 10 minutes to correctly solve the 3 chosen levels.

To pass the evaluation, you need to satisfy the following conditions for each of the 3 random levels:

1.  **Full Connectivity**: All machines on the network must be able to ping each other.
2.  **Correct Addressing**: You must use valid IP addresses and netmasks. The IP addresses should be correctly assigned to hosts and networks.
3.  **No IP conflicts**: No two interfaces can have the same IP address in the same broadcast domain.
4.  **Correct Subnetting**: You must use subnets correctly to divide the network and not waste IP addresses.
5.  **Default Gateway**: The default gateway for each host must be set correctly to allow communication with other subnets.

The project is successfully passed when all 3 random levels are correctly configured and validated by the evaluator within the 10-minute time limit.
