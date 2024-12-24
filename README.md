# Fog-Based Video Processing with Pareto and ACO

## Project Overview
This project demonstrates a fog computing-based system for detecting the presence of the red color in a video stream. By leveraging Docker containers, OpenCV for image processing, Pareto optimization for fog node selection, and Ant Colony Optimization (ACO) for task offloading, this project ensures efficient task offloading and processing across a distributed fog network.

---

## Key Features
- **Real-Time Video Processing**: Uses OpenCV to analyze video frames and detect the presence of red color.  
- **Task Segmentation**: Each video frame is converted into a byte stream and treated as an individual task.  
- **Distributed Fog Network**: Deploys three fog nodes using Docker containers.  
- **Fog Node Selection**: A Pareto optimization approach determines the most suitable fog head for task processing.  
- **Task offloading**: The selected fog head uses Ant Colony Optimization (ACO) to distribute tasks across other fog nodes effectively.

---

## Architecture
1. **Video Frame Processing**:
   - The video is recorded using a camera.
   - Each frame is analyzed for the presence of red color.  
   - If red is detected, the system outputs "Red Detected."

2. **Fog Node Deployment**:
   - Docker containers simulate three fog nodes for distributed task processing.  

3. **Fog Head Selection**:
   - Pareto optimization is used to evaluate and select the optimal fog node to act as the fog head based on parameters like computation capacity, data travel time, and energy usage.  

4. **Task offloading**:
   - The fog head utilizes the ACO algorithm to offload tasks to other fog nodes efficiently.

---



### Hardware
- A system with Docker installed  
- A camera for video input  

---

## How to Run
1. **Set Up Docker Containers**:
   - Deploy three Docker containers to simulate fog nodes.  
   - Configure network settings to enable communication between nodes.  

2. **Start the Video Processing System**:
   - Run the OpenCV-based script to capture video frames and detect the red color.  
   - Ensure frames are converted into byte streams for task distribution.  

3. **Run Fog Node Selection**:
   - Use the Pareto optimization algorithm to identify the most suitable fog head.  

4. **Task offloading**:
   - Deploy the ACO-based task scheduler on the fog head to offload tasks to other fog nodes.  

5. **Monitor Output**:
   - Check the logs for task assignments and confirmation of red color detection.as we can also see where the present task is offloaded to which node and also the processing results using .html files for representation 
..
---


