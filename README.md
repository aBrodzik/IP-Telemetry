# IP-Telemetry

This project was created as a part of my BSc engeenering thesis, that covers the IP telemetry solutions and is based on a virtual test environment. This environment was created using Containerlab. IP network consisting of three autonomous systems was designed to test the capabilities of IP telemetry. Each AS consisted of SR Linux routers and one Alpine Linux client. Each element of the network was virtualized using Docker containers. OSPF and BGP were configured on the routers. Next telemetry tools (gNMIc, Prometheus database, Grafana data visualizer) were added to the created network. The use of telemetry tools made it possible to stream data from routers and visualize them graphically as presented in screenshots below.

# Deployment

- Build clients image from Dockerfile
- Start containerlab with ./start.sh
- Deploy clab: clab-telemetry.yml
- Grafana acces: http://localhost:3000

# Flow Graphs

![g-flows](https://user-images.githubusercontent.com/80266811/219439087-930d4088-100c-489b-8100-d3c57f2024a6.png)
![g-flows-ping](https://user-images.githubusercontent.com/80266811/219439082-0ce1144f-9c5e-4c74-bd65-356657cec631.png)
![flow-iperf](https://user-images.githubusercontent.com/80266811/219438913-b0f044b3-d378-40af-af85-d32005c7ee68.png)

# BGP Graph
![g-bgp](https://user-images.githubusercontent.com/80266811/219439021-c9a5d01c-6ace-4404-a413-98b19653754f.png)
![g-bgp-2](https://user-images.githubusercontent.com/80266811/219439012-36e1e31e-940c-43a5-90b9-31fd26529074.png)

#OSPF Graph
![g-ospf](https://user-images.githubusercontent.com/80266811/219439625-ea5391d1-6d57-4f37-b74e-534bd6e1f860.png)
![g-ospf-2](https://user-images.githubusercontent.com/80266811/219439607-6adf6257-3725-4e46-92df-dd77cc4b518a.png)

![g-routes](https://user-images.githubusercontent.com/80266811/219439161-f0036fc2-8ce8-4ee2-ab56-32d17b66f67a.png)
![g-system](https://user-images.githubusercontent.com/80266811/219439170-9a04cdc7-3f0e-4376-88c4-8d625f5626a0.png)

![g-as1](https://user-images.githubusercontent.com/80266811/219439202-b1310adb-82d9-4e90-9712-536f40a6b164.png)

![g-main-i](https://user-images.githubusercontent.com/80266811/219439275-60e9a929-da67-4282-8137-d15b5ab26f9e.png)
![g-main-a](https://user-images.githubusercontent.com/80266811/219439279-2911b0ca-5939-4689-a3b8-bc413b8a2b9f.png)


#Inspired by
https://github.com/srl-labs/nokia-segment-routing-lab.git
