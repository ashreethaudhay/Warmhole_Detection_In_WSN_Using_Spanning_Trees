# Wormhole Detection in WSN Using Spanning Trees

This project implements a wormhole detection algorithm for wireless sensor networks using spanning trees. It allows generating sensor networks with different deployment models and communication models, inserting wormholes into the networks, and then detecting the wormholes.

## Files
- _network_deployment.py_: Functions to generate sensor network topologies with random, grid, UDG, and QUDG models
- _insert_wormhole.py_: Functions to insert different types of wormholes into a network
- _detect_wormhole.py_: Main wormhole detection algorithm implementation

## Algorithm
The detection algorithm works by choosing multiple root nodes and calculating the variance in shortest path distances when each node is temporarily removed. Wormhole nodes have a higher variance compared to normal nodes. Candidate wormholes are detected by thresholding the variance, and then filtered to only keep connected components of candidates.

## Customizing
The network generation and wormhole insertion functions can be customized or replaced to test the detection on different types of networks.

New detection algorithms can also be implemented and tested on the generated networks with wormholes.

## References
This implementation is based on the algorithm described in the paper:
- WFIND: An Efficient Algorithm for Detecting Wormholes in Wireless Sensor Networks
