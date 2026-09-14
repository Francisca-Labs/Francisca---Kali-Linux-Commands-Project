# Assignment 1 Kali Linux – System Information and Networking

This project demonstrates practical **system information and networking activities performed using Kali Linux**. It covers Linux system identification, hardware and resource monitoring, internet connectivity testing, DNS resolution, and analysis of network round-trip times. 

## Table of Contents

* Project Overview
* Network Topology
* Tools and Technologies
* Configuration Steps
* Results and Findings
* Author

## Project Overview

The purpose of this project was to develop practical knowledge of **Linux system information and basic networking** using a Kali Linux environment.

The assignment focused on using command-line tools to gather system information and perform network connectivity tests, including:

* Identifying the logged-in user and machine hostname
* Determining the current working directory
* Checking Linux kernel information
* Reviewing CPU and RAM information
* Checking available disk space
* Checking system uptime
* Testing internet connectivity
* Testing DNS resolution
* Comparing network round-trip times

## Network Topology

The networking activities were performed from a **Kali Linux virtual machine** connected to the internet.

The network testing involved:

* **Kali Linux VM** as the source system
* **Google Public DNS server:** `8.8.8.8`
* **Google domain:** `google.com`
* **Resolved Google IP address:** `142.250.69.142`

The project used `ping` to test connectivity to the Google Public DNS server and to test connectivity and DNS resolution for `google.com`. 

## Tools and Technologies

* **Kali Linux**
* **Kali Linux virtual machine**
* **Linux command line**
* `whoami`
* `hostname`
* `pwd`
* `uname -a`
* `lscpu`
* `free -h`
* `df -h`
* `uptime`
* `ping`
* **Google Public DNS** (`8.8.8.8`)
* **DNS resolution**

## Configuration Steps

1. Opened the **Kali Linux virtual machine**.

2. Used `whoami` to identify the currently logged-in user.

3. Used `hostname` to identify the machine hostname.

4. Used `pwd` to determine the current working directory.

5. Used `uname -a` to obtain full Linux kernel and system information.

6. Used `lscpu` to review CPU information.

7. Used `free -h` to check RAM usage.

8. Used `df -h` to check disk space by partition.

9. Used `uptime` to determine how long the system had been running.

10. Used `ping -c 2 8.8.8.8` to test basic internet connectivity to the Google Public DNS server.

11. Used `ping -c 4 google.com` to test internet connectivity and DNS resolution.

12. Compared the round-trip times from the two `ping` tests. 

## Results and Findings

The system-information commands successfully provided details about the Kali Linux environment.

* The logged-in username was **`kali`**.
* The machine hostname was **`Kali`**.
* The current working directory was **`/home/kali`**.
* The recorded Kali Linux kernel version was **6.19.14 + Kali amd64**.
* The virtual machine had **1.9 GiB of RAM**.
* Available disk space on the main partition was **889 MB**.
* The recorded system uptime was **13:42:35**.  

The network tests produced the following findings:

* `ping -c 2 8.8.8.8` recorded an average round-trip time of **89.329 ms** with **0% packet loss**.
* `ping -c 4 google.com` successfully resolved `google.com` to **142.250.69.142**.
* The assignment recorded an RTT of **1068 ms** for `8.8.8.8` and **3018 ms** for `google.com`.
* The difference in RTT was attributed to factors including **DNS resolution overhead, routing, latency, and differences in packet-count calculations**. 

Overall, the project provided hands-on experience with **Kali Linux system administration, system monitoring, network connectivity testing, DNS resolution, and basic network troubleshooting**.

## Author

**Ogochukwu Francisca Kelvin-Nwaigwe**

* **Field:** Governance, Risk & Compliance (GRC)
* **School:** Centennial College
* **Location:** Toronto, Canada
* **Career Goal:** **GRC Analyst**
* **LinkedIn:** https://www.linkedin.com/in/francisca-kelvin-nwaigwe/
* **Email:** franciscakelvinnwaigwe@gmail.com
