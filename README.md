# JMeter Performance Test – dMoney API Simulation

## Project Summary:
This project simulates a money transaction system using Apache JMeter and the dMoney API. The scenario is structured into three transaction types, each handled by a dedicated thread group in JMeter:
- **5 agents** perform deposits for **10 customers**
- **5 customers** send money to **10 other customers**
- **5 customers** make payments to **2 merchants**

## Technology:
- Apache JMeter

## Prerequisite:
- Install Java JDK 8+
- Install Apache JMeter 5.5+

## How to run?
### 1. Run Test from GUI (for debugging)
- Open Apache JMeter
- Load `dmoney.jmx`
- Click **Start**

### 2. Run Load Test (Headless)
- jmeter -n -t .\dmoney.jmx -l .\dmoney.jtl -e -o Reports

## Generated HTML reports
![image](https://github.com/user-attachments/assets/47a622d9-19f8-409e-9892-15d142f283ed)


