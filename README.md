# HyperSDK Project

Welcome to the **HyperSDK Project**, a robust and extensible framework designed for blockchain development. This project demonstrates the functionalities of creating, minting, and trading digital assets on a chain using the HyperSDK.

---

## **Table of Contents**

1. [Introduction to the Chain](#introduction-to-the-chain)  
2. [What is HyperSDK?](#what-is-hypersdk)  
3. [Installation Steps](#installation-steps)  
4. [Usage and Examples](#usage-and-examples)  
5. [Contributing](#contributing)  
6. [License](#license)  

---

## **Introduction to the Chain**

This project demonstrates the following core functionalities:  
- **CreateAsset**: Enables the creation of new digital assets on the chain.  
- **MintAsset**: Facilitates minting additional units of an existing asset.  
- **TradeAsset**: Provides the ability to trade digital assets seamlessly within the chain.  

The chain built with HyperSDK is optimized for performance and scalability, making it an excellent foundation for blockchain applications.

---

## **What is HyperSDK?**

HyperSDK is a high-performance toolkit for blockchain development. It simplifies the creation of custom chains by providing pre-built modules, tools, and an extensible framework that supports advanced features like:  
- Asset management  
- Transaction handling  
- Smart contract integration  

With its modular architecture, HyperSDK accelerates development while maintaining flexibility and customization.

---

## **Installation Steps**

Follow these steps to set up and run the HyperSDK project locally:

### **1. Prerequisites**
Ensure the following are installed on your system:  
- **Go** (latest version recommended)  
- **Bash** or any Unix-like shell  

### **2. Setting Up Environment Variables**
Add Go to your system's path. Run one of the following commands based on your setup:  
```bash
export PATH=$PATH:$(go env GOPATH)/bin
```
If the above command does not work, try:  
```bash
export PATH=$PATH:/usr/local/go/bin
```

### **3. Running the Virtual Machine**
Run the following command to start the VM locally:  
```bash
MODE="run-single" ./scripts/run.sh
```

### **4. Building the Project**
Build the project using:  
```bash
./scripts/build.sh
```
> **Note**: If you encounter a "permission denied" error, use the `bash` command to execute the scripts:  
> ```bash
> bash ./scripts/run.sh  
> bash ./scripts/build.sh  
> ```

### **5. Importing Demo Keys**
Use the included demo private key to load default configurations:  
```bash
./build/token-cli key import demo.pk
./build/token-cli chain import-anr
```

---

## **Usage and Examples**

Once the setup is complete, you can explore the functionalities:  

- **Creating an Asset**:  
  Use the `CreateAsset` functionality to define new digital assets.  
  ```bash
  ./build/token-cli action create-asset
  ```

- **Minting an Asset**:  
  Add more units to an existing asset.  
  ```bash
  ./build/token-cli action mint-asset
  ```

- **Trading Assets**:  
  Trade assets within the chain environment.  
  ```bash
  ./build/token-cli action create-order
  ```

---

## **Contributing**

We welcome contributions to improve and extend this project. If you'd like to contribute:  
1. Fork the repository.  
2. Create a new branch for your changes.  
3. Submit a pull request describing your updates.  

For more detailed guidelines, please refer to the [CONTRIBUTING.md](CONTRIBUTING.md) file.

---
