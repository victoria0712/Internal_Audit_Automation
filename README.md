# PO-HC Manager


## Table of contents

- Confidentiality
- Description
- Installation
- Usage
- Features


## Confidentiality

Welcome to the project documentation. In accordance with the commitment to confidentiality, certain sensitive information, including the company name, will not be disclosed within this documentation. The data presented here has been randomly generated for illustrative purposes, ensuring the protection of proprietary details. The documentation showcases the project's capabilities while upholding the principles of confidentiality and security.


## Description

PO-HC Manager was built to automate the process of tracking purchase orders for risk control, resulting in a 300% increase in process efficiency.

One of the primary risks is related to unprocessed purchase orders due to staff turnover. When team members depart without closing their purchase orders, it can lead to operational bottlenecks and potential financial discrepancies. Additionally, newly onboarded team members who initiate purchase orders before completing internal training pose a risk to accuracy and compliance.

To counter these challenges, PO-HC Manager focuses on optimizing purchase order management and minimizing associated risks for Sales Audit Specialists in Sales & Marketing Business Unit Finance Team. By introducing an automated purchase order tracking system, Sales Audit Specialists proactively address the risk of unprocessed orders. This intelligent system ensures that purchase orders are diligently tracked and managed even during transitions, mitigating operational bottlenecks.


## Installation

Pre-requisiste software:
1. Visual Studio

Follow the below steps to run the PO-HC Manager:
1. Download the folder Internal Audit Automation
2. Open Visual Studio 
3. Open the folder Internal Audit Automation
4. Run the first cell to install required packages including XlsxWriter, pandas, numpy, and matplotlib


## Usage

Parameters require changes in the second cell
1. selected_quarter: the quarter period the user would like to know in the format of YYYY QQ. For example, '2021 Q2'
2. top_k: the number of cost centers with largest amount of purchase orders you would like to know. The default is 15.
3. headcount_file_1: headcount file name for the first month in the quarter. For example, '202103HC.csv'
4. headcount_file_2: headcount file name for the last month in the quarter. For example, '202106HC.csv'
5. purchaseoder_file_1: purchase order file name for the previous quarter. For example, 'PO Details2021Q1.csv'
6. purchaseoder_file_2 = purchase order file name for the selected quarter. For example, 'PO Details2021Q2.csv'

Download data
1. Go to the data owner to download the data
2. Put the files in the "input data" file
3. Name the files the same name as you put in the parameters (refer to line 38-41)

Run each cell


## Features

The system is capable of generating:

Graphs
1. PO_num.jpg: Number of Purchase Order by Cost Centers in the selected_quarter
2. PO_total$.jpg: $ Sum of Purchase Order by Cost Centers in the selected_quarter
3. HC_in_out.jpg: Headcount in & out in the selected_quarter

Reports
1. 2021 Q2_HC & PO report.xlsx: master file that shows purchase orders under risk in the first tab, PO to be tracked; new staffs in the second tab, Headcount_in; departing staffs in the third tab, Headcount_out
2. Headcount_In.csv: detailed information for new staffs in the selected quarter
3. Headcount_Out.csv: detailed information for departing staffs in the selected quarter
4. Risk Potential PO.csv: detailed information for departing staffs who left open purchase orders
5. Training List.csv: detailed information for new staffs who open purchase orders frequently


