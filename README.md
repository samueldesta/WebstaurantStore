# WebstaurantStore Outlet Load Test

## Overview
JMeter load test for WebstaurantStore Scratch and Dent Outlet
product pages. Runs at a maximum of 5 RPM for 15 minutes using
randomized product page sampling via a Groovy script.

## Files
- `webstaurantstore_Random_product.jmx` — JMeter test plan
- `Product_Id.csv` — Outlet product IDs and names

## Prerequisites
- Apache JMeter 5.6.3 or higher
- Java installed

## Setup & How to Run
1. Clone this repository
2. Place both files in the same folder
3. Open JMeter
4. File → Open → select `webstaurantstore_Random_product.jmx`
5. Click the Play button
6. Let the test run for 15 minutes (900 seconds)

## Test Configuration
- Duration: 15 minutes (900 seconds)
- Max Throughput: 5 RPM
- Threads: 1 virtual user
- Sampling: Randomized product pages using JSR223 Groovy PreProcessor
- The Groovy script dynamically picks a random product ID and
name from Product_Id.csv each iteration


