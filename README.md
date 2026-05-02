# Multi-Stage Fuel Supply Chain Optimization

This project formulates and solves a multi-stage fuel supply chain optimization problem using Python and PuLP. The model minimizes total system cost across a network of ports, refineries, intermediate warehouses, and final demand nodes.

## Project Overview

The supply chain includes:

- Crude oil transportation from ports to refineries
- Conversion of crude oil into gasoline
- Gasoline transportation through intermediate and final warehouses
- Refinery activation decisions
- Private carrier assignment scenarios
- Demand, disruption, cost, and emissions scenarios

## Optimization Approach

The base model is a linear transshipment optimization problem. Some extensions use binary variables for refinery activation and carrier assignment, making the implemented model a Mixed-Integer Linear Programming formulation.

## Scenarios Evaluated

- Base case
- Refinery shutdown
- Port C supply limitation
- Single private carrier
- Route-by-route carrier assignment
- Company 1 bonus
- Demand shock
- Gasoline transportation cost increase
- Emissions trade-off

## Repository Structure

```text
.
├── fuel_supply_chain_optimization_notebook.ipynb
├── requirements.txt
├── fuel_distribution_results.xlsx
└── figures/