
# Energy Utilization and Optimization Using Advanced Analytics and Machine Learning
This project explores how **data analytics** and **machine learning** can improve the efficiency of cloud systems. It applies:

- **Descriptive analytics** to understand past system performance  
- **Predictive analytics** to anticipate future patterns and potential issues  
- **Prescriptive analytics** to recommend better ways to manage resources  

Machine learning models are used to identify patterns, optimize resource allocation, and make data-driven decisions for energy savings and system efficiency.

The goal is to improve performance, reduce delays, and use energy more effectively, especially in environments that need to scale reliably.

## Background

Cloud service providers are under pressure to deliver high-performance infrastructure while keeping energy use and costs under control. As more businesses move their operations to the cloud, data centers are consuming more energy than ever.

This rise in energy demand leads to:

- Higher carbon emissions  
- Increased operational costs  

This project explores these issues using a dataset that includes performance metrics from a simulated cloud computing environment.

#### Key Challenges

- High energy consumption  
- Inefficient resource use  
- Delayed task execution  

#### Who This Helps

- Businesses that depend on efficient, scalable, and cost-effective cloud services.


## Dataset Overview

![image](https://github.com/user-attachments/assets/c1a1a48e-77e2-4988-8688-c73dc9b61ad2)

#### Attributes

![image](https://github.com/user-attachments/assets/317897df-e1fc-4fba-b4bd-63ad333e3b71)

#### Derived Attributes


- **Energy Efficiency Ratio (EER)** : The **Energy Efficiency Ratio (EER)** measures the energy efficiency of a system by comparing power consumption with the number of executed tasks. A lower EER indicates that the system is using less energy to complete each task, which directly contributes to improved energy efficiency. By reducing the EER, businesses can minimize energy usage, lower operational costs, and promote sustainability, all of which are critical to optimizing cloud computing environments.

   `EER = Power consumption ÷ executed instructions`

- **Sustainability Index (SI)** :  The **Sustainability Index (SI)** is a comprehensive metric that reflects the overall sustainability of a system. It takes into account key factors such as CPU usage, energy consumption, and execution time. A higher SI indicates that the system is performing efficiently with a reduced environmental impact. This metric helps businesses evaluate and improve their cloud operations, aligning them with sustainability goals while ensuring long-term efficiency and performance.

  `SI = (EER × network traffic) ÷ (power consumption + execution time)`

#### Focused Attributes

Key attributes considered in evaluating the environmental impact of cloud performance include **power consumption**, **energy efficiency**, and **network traffic**. **Power consumption** reflects the direct energy demands of workloads, while the **Energy Efficiency Ratio (EER)** highlights how effectively resources are used. **Network traffic** contributes to the **Sustainability Index (SI)**, capturing the link between data transfer and energy use. Correlation analysis shows that both SI and EER have weak relationships with individual resource metrics like **CPU** and **memory usage**, indicating that sustainability is shaped by broader system behavior rather than isolated factors.

![image](https://github.com/user-attachments/assets/71a5cbd0-7642-409a-9602-ae5806119b10)




