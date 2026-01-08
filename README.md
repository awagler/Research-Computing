# HPC Repository for New Mexico State University

Welcome to the High-Performance Computing (HPC) resource repository for **New Mexico State University**. This repository provides documentation, job submission templates, and example workflows to help you get started with HPC resources.

***

## **📌 Quick Start Guide**

### **1. Accessing the HPC Cluster**

*   **Login via SSH:**
    ```bash
    ssh your_username@nmsu.edu
    ```
*   **VPN Requirement:**  
    If you are off-campus, connect to the university VPN before SSH.

***

### **2. Setting Up Your Environment**

*   **Load Modules:**
    ```bash
    module avail        # List available modules
    module load python/3.10
    ```
*   **Using Conda:**
    ```bash
    conda env create -f env/conda-environment.yml
    conda activate hpc-env
    ```

***

### **3. Submitting a Job**

*   **SLURM Example:**
    ```bash
    sbatch scripts/slurm/basic.sh
    ```
*   **Check Job Status:**
    ```bash
    squeue -u your_username
    ```

***

### **4. Transferring Data**

*   **Using SCP:**
    ```bash
    scp localfile.txt your_username@nmsu.edu:/path/to/destination
    ```
*   **Using Globus:**  
    Refer to docs/data-transfer.md.

***

### **5. Documentation**

*   Full user guide: docs/index.md
*   FAQs: docs/faq.md

***

## **Repository Structure**

    hpc-repo/
    ├── docs/        # Documentation
    ├── scripts/     # SLURM/PBS job scripts
    ├── examples/    # Example workflows
    ├── env/         # Environment files
    └── ci/          # CI/CD configuration

***

## **Contributing**

See CONTRIBUTING.md for guidelines.

***

## **License**

This repository is licensed under LICENSE.


