# SMC Service Blueprint

This repository provides a reference architecture and API specification for building a **generic Secure Multiparty Computation (SMC) service**. It is intended to serve as a blueprint for building privacy-preserving, interoperable, and SMC services across untrusted or semi-trusted parties, with centralized orchestration.

This repo focuses on presenting a modular architecture for SMC Services and strictly define aspects of the infrastructure that are not use-case-specific.

## Repository Structure

| Path             | Description                                      |
|------------------|--------------------------------------------------|
| `docs/`          | Core design specification                        |
| `api/`           | API specification                                |
| `docker/`        | Dockerized utilities                             |

## Key Components

### Architecture

See [`docs/architecture.md`](docs/architecture.md) for a full specification of the service architecture.

### API Specification

An [OpenAPI](https://www.openapis.org/) definition of the base Computation Node API is available in `api/cn/`. 

It can be previewed locally via Swagger UI using, for example, the provided docker compose:
```bash
cd docker/
docker compose up swagger-ui
```

## Useful Resources

- [MP-SPDZ](https://github.com/data61/MP-SPDZ)  
    A state-of-the-art framework for SMC protocols and implementations.
- [QMP-SPDZ](https://github.com/diogoftm/QMP-SPDZ)  
    MP-SPDZ fork with a quantum-enabled version implementation of SMC protocols based on Oblivious Transfer leveraging quantum oblivious keys.
- [Generation and Distribution of Quantum Oblivious Keys for Secure Multiparty Computation](https://www.mdpi.com/2076-3417/10/12/4080) <br>
    Research paper with an overview of the main concepts behind quantum oblivious keys. 

## Acknowledgments

We acknowledge the support of:
- The QuantaGenomics project funded within the QuantERA II Programme that has received funding from the European Union's Horizon 2020 research and innovation programme under Grant Agreement No 101017733, and with funding organizations, the Foundation for Science and Technology – FCT (QuantERA/0001/2021), Agence Nationale de la Recherche - ANR, and State Research Agency – AEI.
- The QSNP project that has received funding from the European Union's Horizon Europe research and innovation programme under the project "Quantum Security Networks Partnership" (QSNP, grant agreement No 101114043).
