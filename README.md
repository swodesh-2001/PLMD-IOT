# Predictive Load Management Using Advanced Data Analytics 
 
  - [Introduction](#introduction)
  - [Problem Statements](#problem-statements)
    - [Increasing Energy Demand](#increasing-energy-demand)
    - [Infrastructure Limit](#infrastructure-limit)
    - [Uneven Demand](#uneven-demand)
    - [Inaccurate/No Historical Data](#inaccurateno-historical-data)
  - [Concept of Smart Grid](#concept-of-smart-grid)
  - [Predictive Load Management Device (PLMD)](#predictive-load-management-device-plmd)
  - [Decentralized Demand Flattening](#decentralized-demand-flattening)
  - [Load Categorization](#load-categorization)
  - [Dynamic Tariff Structure](#dynamic-tariff-structure)
  - [Advantages](#advantages)
  - [Conclusion](#conclusion)
  - [Prediction Demo](#prediction-demo)
  - [Load Scheduling](#load-scheduling)
  - [What Does PLMD Do?](#what-does-plmd-do)
  - [How Energy Demand is Predicted](#how-energy-demand-is-predicted)
- [References](#references)
- [Training History](#training-history)
- [RNN Network Architecture](#rnn-network-architecture)


### Introduction

**Demand Side Management:**

- Manage the demand for electricity in the power grid.
- Aims to optimize the use of electricity, reduce peak demand, and improve the overall efficiency of the power system.
- Helps to reduce the need for new power plants and other infrastructure.
 

### Problem Statements

#### Increasing Energy Demand

- High demand in winter season and peak hours.
- Importing electricity from neighboring countries.
- If unable to fulfill the demand then load shedding and blackouts.

![Image](./images/slide_4_image_1028.png)

---

#### Infrastructure Limit

- Lack of water reservoir which leads to importing electricity in peak hours (which is expensive).
- Lack of two-way communication between utility and consumer.

![Image](./images/slide_5_image_167.png)

---

#### Uneven Demand

- Energy consumption is less in off-peak hours (Peak/average ratio is less).
- Consumers consume more electricity during morning and evening times of the day.

![Image](./images/slide_6_image_12.png)

---

#### Inaccurate/No Historical Data

- Accurate and comprehensive data on past electricity consumption patterns is crucial for understanding current demand patterns and forecasting future demand.

![Image](./images/slide_7_image_192.png)

---

### Concept of Smart Grid

- All the renewable sources to the grid.
- Real-Time Monitoring.
- BEM using various DSM techniques.
- Incentivizing Consumers.

![Image](./images/slide_8_image_201.png)

---

### Predictive Load Management Device (PLMD)

![PLMD](./images/PLMD.png)

- Real-time energy consumption.
- Future demand prediction.
- Renewable integration during peak hours.
- Load scheduling and tariffs development.
- Dataset generation.

---

```mermaid
graph TD
    A[Real-time Energy Consumption] --> B[Future Demand Prediction]
    A -.-> C[Dataset Generation]
    C -.-> B
    B --> D[Renewable Integration During Peak Hours]
    B --> E[Load Scheduling and Tariffs Development]
```

![PLMD2](./images/whole_setup.png)

**Hardware**
<div style="display: flex; justify-content: space-between; margin-top: 20px;">
  <img src="./images/hardware1.png" alt="hardware1" style="width: 48%;">
  <img src="./images/hardware2.png" alt="hardware2" style="width: 48%;">
</div>

### Decentralized Demand Flattening

<div style="display: flex; justify-content: space-between;">
    <img src="./images/lstm.png" alt="Image 1" style="width: 70%">
    <img src="./images/mobile.png" alt="Image 2" style="width: 25%;">
</div>

 ![Data_prediction](./images/charts.png)

---

### Load Categorization

 ![Load Categorization](./images/Load_categorization.png)

---

### Dynamic Tariff Structure

![tarrif](./images/Tarrif_structure.png)
 

---

### Advantages

- Helps to ensure the availability of enough capacity to meet tomorrow’s demand.

<div style="display: flex; justify-content: space-between;">
    <img src="./images/slide_18_image_264.png" alt="Image 1" style="width: 48%;">
    <img src="./images/slide_18_image_265.png" alt="Image 2" style="width: 48%;">
</div>

- Automatic integration of renewable energy sources (if available).
<div style="display: flex; justify-content: space-between;">
    <img src="./images/slide_18_image_268.png" alt="Image 1" style="width: 48%;"> 
</div>
 

---

- Hides the complexity of DSM from the users and creates a user-friendly interface.
<div style="display: flex; justify-content: space-between;">
    <img src="./images/slide_19_image_278.png" alt="Image 1" style="width: 48%;"> 
</div>
 

- Utilizes the leftover inverter batteries bought during the previous blackout and automates it.


<div style="display: flex; justify-content: space-between;">
    <img src="./images/slide_19_image_280.png" alt="Image 1" style="width: 40%;">
    <img src="./images/slide_19_image_281.png" alt="Image 2" style="width: 48%;">
</div>

---
 
### Conclusion

- Demand Prediction
- Deferrable Load Scheduling
- Automatic Renewable Integration
- Eliminates DSM complexity from user


### Prediction Demo

![demo](./images/demo.gif)

https://user-images.githubusercontent.com/70265297/211731263-cf6aa78a-02fa-447f-be15-22387b881e76.mp4


### Load Scheduling

```mermaid
flowchart TD
    A[START] --> B[RUN HIGH PRIORITY APPLIANCE]
    B --> C{RE AVAILABLE?}
    C -->|YES| D[SCHEDULE MIDDLE AND LOW ORDER APPLIANCE ACCORDING TO RE AVAILABILITY]
    C -->|NO| E[STOP LOW AND MIDDLE ORDER APPLIANCE]
    D --> F[STOP]
    E --> F[STOP]

```
---

### What Does PLMD Do?

- Regularly monitors the real-time energy usage and cloud storing.
- Automatic PV Switching based on peak hours.
- Peak load management, improved QoS, and reliability.
- Simple and user-friendly IoT interface.
- Used as basic energy meter.

![Image](./images/slide_32_image_234.png)


### How Energy Demand is Predicted

- Energy consumption pattern is different for different people but is affected by factors such as:
  - Weather condition
  - Holiday
  - Past consumption pattern
  - Festivals

<div style="display: flex; justify-content: space-between;">
  <img src="./images/slide_33_image_7.png" alt="Image" style="width: 32%;">
  <img src="./images/slide_33_image_8.png" alt="Image" style="width: 32%;">
  <img src="./images/slide_33_image_9.png" alt="Image" style="width: 32%;">
</div>

---


## References

- Abdul Hafeez Abid and Ammar Hasan. An approach for demand side management of non-flexible load in academic buildings, IEEE, 2018.
- Isaiah Adediji Adejumobi and Joseph Adesina Adeoti. Efficient utilization of industrial power: demand side management approach, IEEE, 2019.
- SP Anjana and TS Angel. Intelligent demand side management for residential users in a smart micro-grid, IEEE, 2017.
- Wan He. Load forecasting via deep neural networks. Procedia Computer Science, 122:308–314, 2017.
- K Maharaja, P Pradeep Balaji, S Sangeetha, and M Elakkiya. Development of bidirectional net meter in grid connected Solar PV system for domestic consumers. In 2016 International Conference on Energy Efficient Technologies for Sustainability (ICEETS), pages 46–49. IEEE, 2016.
- Asha Radhakrishnan and MP Selvan. Load scheduling for smart energy management in residential buildings with renewable sources. In 2014 Eighteenth National Power Systems Conference (NPSC), pages 1–6. IEEE, 2014.
- Judith Stute and Matthias Kühnbach. Dynamic pricing and the flexible consumer–investigating grid and financial implications, 2023.

---


## Training History

![Image](./images/slide_15_image_317.png)

## RNN Network Architecture

![Image](./images/slide_15_image_319.png)
 




 
