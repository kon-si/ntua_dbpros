# Advanced Topics in Database Systems

## Table of contents
* [Team Information](#team-information)
* [Specifications of VMs used](#specifications-of-vms-used)
* [Technologies](#technologies)
* [Setup](#setup)
* [Dataset](#dataset)

## Team Information
Team Code on Helios: 92
Team Members: 
Christina Diamanti
Konstantinos Sideris

## Specifications of VMs used:
For this project we used two Virtual Machines, one had the role of the Master and the other of the Slave. Each VM was assigned with an IPv6 address, and the Master was also assigned a public IPv4 address. The two VMs communicate over an IPv4 local network. 

| OS  |  CPUs | RAM | Disk space | 
| ------------- |  ------------- | ------------- | ------------- |
| Ubuntu 18.04.6 LTS  | 4 |  8GB | 30GB | 

| VM  |  Local Net IPv4 |
| ------------- |  ------------- |
| Master  |  192.168.0.1 | 
| Slave  |  192.168.0.2 | 

## Technologies 
Project is created with:
* Apache Hadoop 3.3.4
* Apache Spark 3.3.1
* Scala 2.13.10
* SBT 1.8.2

## Setup 

## Dataset
The Dataset used for this project is the [TLC Trip Record Data](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page). 
More specifically we used data from the Yellow Taxi Trip Records for the months of January to June of 2022. All taxi trip records were in parquet format. We also used the taxi zone lookup csv file found in this [link](https://d37ci6vzurychx.cloudfront.net/misc/taxi+_zone_lookup.csv), which we needed to be able to connect LocationID information with the name of the zone of the Location.
Yellow taxi trip records include fields capturing pick-up and drop-off dates/times, pick-up and drop-off locations, trip distances, itemized fares, rate types, payment types, airport fees, and driver-reported passenger counts.
