# Automotive Technical Publication: Front Disc Brake Caliper Service Manual

An engineering service manual and Illustrated Parts Catalog (IPC) authored using **DITA XML 1.3** and formatted in accordance with **ASD-STE100 (Simplified Technical English)** standards.

---

## 📌 Project Overview
This project demonstrates modular technical authoring workflows commonly used by engineering service providers (such as LTTS, Tata Technologies, Cyient, and Quest Global) to create maintenance documentation and spare parts catalogs for automotive and aerospace OEMs.

* **Target Assembly:** Single Piston Floating Caliper Assembly
* **Document Number:** DOC-BRK-2026-01
* **Standards Followed:** ASD-STE100, OASIS DITA XML 1.3 Architecture
* **Primary Output:** Formatted PDF Service & Parts Manual

---

## 🗂️ Content Architecture (DITA XML)
The documentation follows topic-based authoring principles separating content into modular components:

* **Concept Topic (`dita/concept_disc_brake.dita`):** Explains system operation, hydraulic actuation, and key service wear specifications.
* **Task Topic (`dita/task_brake_pad_replacement.dita`):** Provides step-by-step removal, inspection, and installation procedures authored in Simplified Technical English with explicit safety warnings and torque specifications.
* **Reference Topic (`dita/reference_ipc_disc_brake.dita`):** Defines the Illustrated Parts Catalog (IPC) with exploded assembly callouts and a structured Bill of Materials (BOM) table.
* **DITA Map (`dita/brake_manual.ditamap`):** Acts as the publication manifest binding the concept, task, and reference files into a unified document structure.

---

## 📂 Repository Structure
```text
brake-caliper-service-manual/
├── dita/
│   ├── brake_manual.ditamap             # Table of contents & publication map
│   ├── concept_disc_brake.dita          # System overview & technical specs
│   ├── task_brake_pad_replacement.dita  # Maintenance SOP (STE compliant)
│   └── reference_ipc_disc_brake.dita    # Illustrated Parts Catalog (IPC & BOM)
├── images/
│   └── fig1_exploded_view.gif           # Exploded view diagram with balloon callouts
└── output/
    ├── service_manual.html              # Structured HTML print source
    └── Front_Brake_Caliper_Service_Manual.pdf # Final published manual