
# Monitoring Website and server using Prometsus an Alert Manager

![alt text](https://github.com/prakhar-mathur4/Monitorig-Project-1/blob/main/MOP.png)

Overview: Implemented a monitoring solution for websites and servers using Prometheus and Alertmanager, ensuring real-time observability, proactive incident detection, and automated alerting


## Tech Stack

**Website:** Java(Springboot), HTML, CSS, JavaScript
**Monitoring Tools:** Prometheus, Alertmanager
**Infrastructure:** 
* **AWS Cloud:** Linux EC2 Instance





## Installation
**1. Setup EC2 Instances:**     
In this project, two EC2 instances were created—one for Prometheus, Alertmanager, and Blackbox Exporter, and another for hosting the website and Node Exporter. The setup process included selecting an appropriate Amazon Machine Image (AMI) such as Ubuntu, choosing an instance type based on resource requirements here i have selected t2.medium, and configuring security groups to allow necessary inbound and outbound traffic.


```bash
ffff
```
    
**2. Install and Run Prometheus:**
Run the following command to download and install Prometheus.

```bash
# Download the prometheus
wget https://github.com/prometheus/prometheus/releases/download/v3.2.0/prometheus-3.2.0.linux-amd64.tar.gz
# Unxip the prometheus
tar -xvf prometheus-3.2.0.linux-amd64.tar.gz
# Remove the Zip file
rm prometheus-3.2.0.linux-amd64.tar.gz
# Rename the prometheus folder
mv prometheus-3.2.0.linux-amd64/ prometheus
# Run Prometheus in background
./prometheus &
```


**3. Install and Run Alert Manager:**
Run the following command to download and install Alert Manager.

```bash
# Download the alertmanager
wget https://github.com/prometheus/alertmanager/releases/download/v0.28.0/alertmanager-0.28.0.linux-amd64.tar.gz
#Unxip the alertmanager
tar -xvf alertmanager-0.28.0.linux-amd64.tar.gz
# Remove the Zip file
rm alertmanager-0.28.0.linux-amd64.tar.gz
# Rename the alertmanager folder
mv alertmanager-0.28.0.linux-amd64/ alertmanager
# Run alertmanager in background
./alertmanager &
```

**4. Install and Run Blackbox Exporter:**
Run the following command to download and install Blackbox Exporter.
```bash
# Download the blackbox_exporter
wget https://github.com/prometheus/blackbox_exporter/releases/download/v0.25.0/blackbox_exporter-0.25.0.linux-amd64.tar.gz
#Unxip the blackbox_exporter
tar -xvf blackbox_exporter-0.25.0.linux-amd64.tar.gz
# Remove the Zip file
rm blackbox_exporter-0.25.0.linux-amd64.tar.gz 
# Rename the blackbox_exporter folder
mv blackbox_exporter-0.25.0.linux-amd64/ blackbox_exporter
# Run blackbox_exporter in background
./blackbox_exporter &
```


----            


Now configure Prometheus, Alert Manager & Blackox exporter

---

## Project Glimpse
![alt text](https://github.com/prakhar-mathur4/Monitorig-Project-1/blob/main/image1.png)
![alt text](https://github.com/prakhar-mathur4/Monitorig-Project-1/blob/main/image2.png)
![alt text](https://github.com/prakhar-mathur4/Monitorig-Project-1/blob/main/image5.png)
![alt text](https://github.com/prakhar-mathur4/Monitorig-Project-1/blob/main/image6.png)
![alt text](https://github.com/prakhar-mathur4/Monitorig-Project-1/blob/main/image8.png)
![alt text](https://github.com/prakhar-mathur4/Monitorig-Project-1/blob/main/image9.png)
