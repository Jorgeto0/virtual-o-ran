# Virtualized Open RAN System on Kubernetes

This repository contains a virtualized Open RAN system running on Kubernetes. The project simulates and tests O-RAN components such as the Central Unit (CU), Distributed Unit (DU), and Near-Real-Time RAN Intelligent Controller (Near-RT RIC) using open-source software.

## Components

### Active Components
- **CU (Central Unit):**
  - Implemented using OpenAirInterface (OAI).
  - Deployed as a containerized application in Kubernetes under the `cu` namespace.
  - All future development and testing will use this CU as the primary implementation.

- **DU (Distributed Unit):**
  - To be implemented using OpenAirInterface (OAI).
  - Will communicate with the CU to handle real-time RAN functions.

- **Near-RT RIC:**
  - The Near-RT RIC will host xApps for real-time RAN optimization.
  - Future implementation planned using the O-RAN Software Community (OSC).

### Archived Components
- **Archived CU:**
  - The original placeholder CU, a simple Flask app used for testing deployments and services, is stored in the `src/components/archived-cu` folder.
  - The associated Kubernetes resources have been deleted, but files remain for reference.

## Folder Structure

```plaintext
src/
├── components/
│   ├── cu/                  # OAI-based Central Unit
│   ├── du/                  # Distributed Unit (to be implemented)
│   ├── near-rt-ric/         # Near-RT RIC (future implementation)
│   ├── archived-cu/         # Placeholder CU for testing (archived)
docs/
├── architecture/            # Architecture diagrams and plans
├── training/                # Training materials for team members
