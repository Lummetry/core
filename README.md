
# Naeural Edge Protocol Core Modules

Welcome to the Naeural Edge Protocol Core Modules repository. These modules form the backbone of the Naeural Edge Protocol framework, a decentralized job execution meta-OS researched under two public financing grants, enabling the creation of end-to-end AI pipelines for edge computing. This README provides an overview of the core functionality, components, and how to get started with the Naeural Edge Protocol.

> Note: this repository does not contain and it is not supposed to provide any kind of CI/CD pipeline. This repository is a development dissemination environment for the meta-OS base framework and it is not intended to be used in production environments.

---

## SOLIS and ReDeN projects disclaimer

This repository is a refactored version of the original open-source project based on SOLIS (SMIS 143488) and ReDeN (SMIS156084) research grant projects and through this refactoring of the original project, we foster a collaborative environment that promotes innovation while respecting intellectual property rights. We look forward to the community's contributions and to advancing the objectives set forth by the SOLIS and ReDeN projects. The refactoring was undertaken to enhance clarity and relevance for non-proprietary business use cases and by restructuring the codebase and removing proprietary components, we aim to provide a more accessible and compliant foundation for community contributions and commercial applications. 


**Originating Projects**

This work builds upon the foundational efforts of two significant research grant projects:

1. **SOLIS** (SMIS 143488)

   - **Description**: The SOLIS project served as the initial source of this codebase. It focused on developing innovative solutions in deep vision based safety and security systems.
   - **Contribution**: SOLIS provided the groundwork for core functionalities and established the primary architecture upon which this repository is built.

2. **ReDeN** (SMIS 156084)

   - **Description**: The ReDeN project aimed to create a decentralized processing network. It expanded upon the work of SOLIS by introducing decentralized methodologies and technologies.
   - **Contribution**: ReDeN enhanced the scalability and robustness of the system, enabling more efficient distributed processing capabilities.

_We gratefully acknowledge the support and contributions of the SOLIS (SMIS 143488) and ReDeN (SMIS 156084) projects. Their pioneering work laid the essential foundation for this repository, and their objectives continue to inspire ongoing development._

---

## Overview

The Naeural Edge Protocol is designed to facilitate the rapid development and deployment of AI applications at the edge. These core modules are responsible for the following key functionalities:

- **Data Collection**: Acquire data via multiple methods, including:
  - Default plugins: MQTT, RTSP, CSV, ODBC
  - Custom-built plugins for sensors and other data sources

- **Data Processing**: Transform and process collected data to prepare it for trustless model training and inference.

- **Model Training and Inference**: Use plugins to train AI models and perform trustless inference tasks.

- **Post-Inference Business Logic**: Run business logic post-inference to derive actionable insights and decisions.

- **Pipeline Persistence**: Ensure the persistence of pipelines for reliability and reproducibility.

- **Communication**: Facilitate communication through MQ-based and API-based methods, including routing and load balancing via ngrok.

These modules can be used as the core for implementing edge nodes within the Naeural Edge Protocol or integrated into third-party Web2 implementations.

## Features

- **Modular Design**: Easily extend functionality with custom plugins for data collection, processing, and more.
- **Scalability**: Designed to scale from small edge devices to large-scale deployments.
- **Interoperability**: Compatible with a variety of data sources and communication protocols.
- **Ease of Use**: Provides low-code/no-code development capabilities for rapid pipeline creation.

### Contributing

We welcome contributions from the community. Please read our [CONTRIBUTING.md](CONTRIBUTING.md) for details on how to contribute to the project.

### Installation

To install the naeural-core package on systems without cuda capabilities, run

```bash
pip install naeural-core
```

To install the naeural-core package on systems with cuda capabilities, run

```bash
pip install naeural-core --extra-index-url https://download.pytorch.org/whl/cu121
```

You can change the cuda driver with the one you already have. (For cuda 11.7, use cu117)

If the installation fails, try to run it again with the flags `--upgrade` and `--force-reinstall`

```bash
pip install naeural-core --upgrade --force-reinstall --extra-index-url https://download.pytorch.org/whl/cu121
```

### License

This project is licensed under the Apache 2.0 License - see the [LICENSE](LICENSE) file for details.

## Contact

For more information, visit our website [https://naeural.ai](https://naeural.ai) or reach out to us at support@naeural.ai.


# Project Financing Disclaimer

This project includes open-source components that have been developed with the support of financing grants SMIS 143488 and SMIS 156084, provided by the Romanian Competitiveness Operational Programme. We are grateful for this support, which has enabled us to advance our work and share these resources with the community.

The content and information provided within this repository are solely the responsibility of the authors and do not necessarily reflect the views of the funding agencies. The funding received under these grants has been instrumental in supporting specific parts of this open source project, allowing for broader dissemination and collaborative development.

For any inquiries related to the funding and its impact on this project, please contact the authors directly.

# Citing

```bibtex
@misc{project_funding_acknowledgment1,
  author       = {Damian, Bleotiu, Saraev, Constantinescu},
  title        = {SOLIS – Sistem Omogen multi-Locație cu funcționalități Inteligente și Sustenabile”
SMIS 143488},
  howpublished = {\url{https://github.com/NaeuralEdgeProtocol/}},
  note         = {This project includes open-source components developed with support from the Romanian Competitiveness Operational Programme under grants SMIS 143488. The content is solely the responsibility of the authors and does not necessarily reflect the views of the funding agencies.},
  year         = {2021-2022}
}
```

```bibtex
@misc{project_funding_acknowledgment2,
  author       = {Damian, Bleotiu, Saraev, Constantinescu, Milik, Lupaescu, Stoica, Balaci},
  title        = {ReDeN – Rețea Descentralizată Neurală SMIS 156084},
  howpublished = {\url{https://github.com/NaeuralEdgeProtocol/}},
  note         = {This project includes open-source components developed with support from the Romanian Competitiveness Operational Programme under grants SMIS 143488. The content is solely the responsibility of the authors and does not necessarily reflect the views of the funding agencies.},
  year         = {2023-2024}
}
```


```bibtex
@misc{PyE2,
  author = {Stefan Saraev, Andrei Damian, Cristian Bleotiu},
  title = {PyE2: Python SDK for Naeural Edge Protocol},
  year = {2024},
  howpublished = {\url{https://github.com/NaeuralEdgeProtocol/PyE2}},
}
```