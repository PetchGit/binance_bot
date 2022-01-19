Hi, My name is Petch. Warm welcome to you.

This module is named OMBB abbreviated from 'One-Page Multimonitor Binance Bot'. I created this module with these two philosophies in mind.

- Structure in a way that is so simplified that even a python beginner can write a full function trading bot all by himself.
- Design philosophy is one trader looks at 150+ tickers at all times. Because, for example, one might trade ETH based on movement in BTC.

This read me file is going to lead you guys through these topics. Feel free to skip ahead if you're looking for a specific one.

---

# Contents

## [How to setup](#how-to-setup)

- Setup Python
- Setup Binance
- Setup OMBB

## [Python 101](#python-101)

- Introduction
- Basic Datastructures
- Commonly Use

## [Use OMBB for Trading](#use-ombb-for-trading)

- Structures
- Commands
- Indicators

## [Use OMBB for Backtesting](#use-ombb-for-backtesting)

- Collect Market Data
- Run a virtual world

## [Use OMBB for Stress Test](#use-ombb-for-stress-test)

- Overview
- Montecarlo Shuffling Simulation
- Montecarlo Resampling Simulation
- Out of Sample Backtesting
- Date Shifting Backtesting

---

# How to setup

## Setup Python

- Install VS Code
- Install Python
- Create Virtual Environment
- Download OMBB
- Install Python Libraries

## Setup Binance

- Get your API key from Binance
- Connect your API key to OMBB

## Setup OMBB

- Create your first strategy
- Live your first Trading Bot

---

# Python 101

## Introduction

- Print
- Basic Variable Types
- Basic Operation
- If/Else Statements
- Loops

## Basic Datastructures

- Strings
- Lists
- Dictionary
- Dataframe

## Commonly Use

- Function
- Import
- Try/Except

---

# Use OMBB for Trading

## Structures

- Create New Strategy
- When/How each method is called
- Set Parameters

## Commands

- Access a Candle Stick
- Send Buy/Sell Orders

## Indicators

- Add an indicator
- Where to look for reference
- Access the indicator value
- Create your own indicator

---

# Use OMBB for Backtesting

## Collect Market Data

- How to run

## Run a virtual world

- How to run
- How to save your result

---

# Use OMBB for Stress Test

## Overview

- How does the worst losing streak look like?
- Comparison to Monkeys Throwing Darts? Treasury Notes? Buy and Hold ?
- Is this result a fluke ?
- Is this over fitting?

## Montecarlo Shuffling Simulation

> A quick and dirty simulation to see what the worst losing streak might look like

## Montecarlo Resampling Simulation

> A quick and dirty simulation to see the profiability robustness.

## Out of sample Backtesting

> Slightly longer backtesting with out-sample data to see the profiability robustness..

## Walk forward Analysis

> Multi-stage approach to optimize parameters that best perform in a specific market regime

## Clustered Walk forward Analysis

> Investigate range of parameters that best perform in a specific market regime

# Thought process on Strategy Creation

- Create Trading Strategy based on 6 areas
  - Identify Market Condition
  - Choose Symbol
  - Entry Condition
  - Exit Condition
  - Stop Loss Condition
  - Position Sizing
  - Account Limit
  - Misc
- Feasibility Analysis
  - Montecarlo Shuffling
    - Worst Drawdown Criteria
  - Montecarlo Resampling
    - Confidence Level Criteria to Profitability
  - Out of sample testing
    - Confidence Level Criteria to Profitability
- Optimization
  - Walk Forward Analysis
    - Find the best parameters from various market regime
    - Optimize less than 3 parameters
    - Optimize ratio 4:1 (optimize phase : forward phase)
  - Clustered Walk Forward Analysis
    - Find range of values that each parameters can perform the best
- Real Money
  - Result Feedback
