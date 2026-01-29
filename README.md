# Small Spiking Network using Izhikevich Neuron Model

## Overview
This project explores how **simple spiking neuron models**, when connected into a network, can give rise to **emergent collective dynamics** such as synchrony, bursting, and population-level activity.

The goal of this work is **conceptual understanding**, not biological completeness.  
All simulations are implemented **from scratch in Python** to better understand the principles of computational neuroscience.

---

## Motivation
While single neuron models are useful for studying individual firing properties, real brain function emerges from **interactions between many neurons**.  
This project investigates how:

- excitation and inhibition,
- random connectivity,
- and external inputs

together shape **network-level spiking behavior**.

This aligns with a core question in computational neuroscience:
> *How do collective neural dynamics arise from simple local rules?*
> *Why are some neurons silent?*
> *Why bursts appear?*
> *What happens if inhibition increases?*

---

## Model Description

### Neuron Model
Each neuron in the network is modeled using the **Izhikevich spiking neuron model**, which balances:
- biological plausibility
- computational efficiency

The model captures diverse firing patterns using only two coupled differential equations.

---

### Network Structure
- Total neurons: **50**
- Composition:
  - 80% excitatory neurons
  - 20% inhibitory neurons
- Connectivity:
  - Random (Erdős–Rényi–like)
  - Both excitatory and inhibitory synaptic effects
- Synapses:
  - Current-based
  - Fixed synaptic weights

This minimal structure is sufficient to study emergent dynamics without unnecessary complexity.

---

## Simulation Details
- Time resolution: discrete time steps (ms scale)
- External input:
  - Random background current to each neuron
- Spikes are detected using a voltage threshold and recorded for analysis

---

## Results

### Raster Plot
The primary output of the simulation is a **raster plot** showing:
- neuron index vs time
- spike timing across the population

This visualization allows observation of:
- synchronous firing events
- burst-like activity
- variability across neurons

Even with simple neuron and synapse models, the network exhibits **non-trivial collective behavior**.

---

## Observations
Some qualitative observations from the simulations include:
- Increasing excitatory drive can lead to synchronized spiking
- Inhibitory neurons play a stabilizing role in network activity
- Network dynamics are sensitive to excitation–inhibition balance

These behaviors emerge **without any learning or plasticity**, highlighting the power of network interactions alone.

---

## Limitations
This model intentionally avoids:
- synaptic plasticity (e.g., STDP)
- spatial structure
- conductance-based synapses

The focus is on **conceptual clarity**, not biological completeness.

---

## What I Learned
Implementing this network helped me understand:
- how population dynamics differ from single-neuron behavior
- why inhibition is crucial for stability
- how simple models can still generate complex dynamics

This project strengthened my interest in **theoretical and computational approaches to neuroscience**.

---

## References
- Izhikevich, E. M. (2003). *Simple model of spiking neurons*. IEEE Transactions on Neural Networks.
- Izhikevich, E. M. (2004). *Which model to use for cortical spiking neurons?*
- Dayan, P., & Abbott, L. F. (2001). *Theoretical Neuroscience*.

---

## Notes
This project is intended as a **learning and exploration exercise** and is part of my preparation for further research training in computational neuroscience.
