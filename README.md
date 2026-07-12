# Cafe Queue Discrete Probability Modeling

## Overview

This project develops a discrete probabilistic simulation model for a café queuing system in R language. Customers arrive randomly, place orders from a 7-item menu, and wait for their orders to be prepared by a dynamic team of servers.

This project demonstrates proficiency in:
- Stochastic Modeling: Applying Poisson, multinomial, and geometric distributions in a real-world simulation context
- Discrete-Event Simulation: Implementing a slot-based simulation engine
- Performance Evaluation: Analyzing queue behavior under various load conditions
- Dynamic Systems: Modeling adaptive server allocation based on state feedback
- Data Visualization: Creating professional plots to communicate results effectively

## Simulation
The simulation captures real-world service dynamics through:
- Stochastic arrival patterns (Poisson process)
- Menu preferences (multinomial distribution)
- Item-dependent preparation times (Geometric distribution)
- Dynamic server allocation (2 base servers + optional 3rd for rush hours)

This model enables analysis of queue behavior, service efficiency, and system performance under varying load conditions.

## Mathematical Model

### Discrete-Time Framework Parameters
- Time Slot: 5 minutes
- Number of arrivals in slot t, with Poisson Distribution
- Queue length at slot boundary after slot t (customers awaiting completion)

### Server Dynamics
- Base Servers: 2 always active
- Third Server: Activated dynamically when the queue length reaches an activation threshold h.
​
### Service Model Parameters
- Service time of a single customer in slots
- Per-slot service success probability (item-specific) with Geometric Distribution
