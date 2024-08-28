# Code for the Confernece Paper "Dynamic Resource Allocation using Second Price Auction in Quantum Cloud Computing" 
# IBM Quantum Setup Guide

This repository provides instructions on how to create an IBM Quantum (IBMQ) account and how to use it in your Python projects. Additionally, an example code snippet is provided to get you started with accessing IBMQ resources.

## Getting Started

### 1. Create an IBM Quantum Account

To use IBM's quantum computers, you'll need an IBM Quantum (IBMQ) account. Follow these steps to create one:

1. Visit the [IBM Quantum Experience](https://quantum-computing.ibm.com/) website.
2. Click on the **Sign Up** button if you don't already have an account. If you have an IBM ID, you can use that to sign in.
3. Fill in the required details and complete the registration process.
4. After registration, log in to your IBM Quantum account.
5. Navigate to your **Account Settings** by clicking on your profile icon in the top-right corner.
6. Under **API Token**, click on the **Copy** button to copy your API token. This token will be used to authenticate your access to IBMQ resources.

### 2. Setting Up the Environment

Before using IBMQ, you'll need to install `qiskit` and set up your Python environment.

1. **Create a Python Virtual Environment:**

   ```bash
   python -m venv myenv
   source myenv/bin/activate  # On Windows, use `myenv\Scripts\activate`
