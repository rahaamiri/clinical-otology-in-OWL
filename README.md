# 🏥 Semantic Clinical Otology

### A Decision Support System for Ear Surgery & Medication Safety

**Author:** Fatemeh Amirkolaei
**Course:** Knowledge Representation
**Tools:** Protégé 5.5, OWL 2 DL, SWRL, HermiT Reasoner, SPARQL

---

## 📖 Project Overview
This project implements a formal ontology for an Otology department to model patient data, surgical procedures, and anatomical structures.

Beyond simple data modeling, this system functions as a **Clinical Decision Support System (CDSS)**. It uses **SWRL (Semantic Web Rule Language)** and an **OWL Reasoner** to automatically infer patient risk categories and detect medical errors (such as drug-allergy interactions) in real-time.

### 🎯 Key Objectives
1.  **Patient Safety:** Prevent medication errors by cross-referencing prescriptions against allergy profiles.
2.  **Automatic Triage:** Classify patients (e.g., *Surgical Patient*, *High Risk*) based on their clinical history without manual input.
3.  **Semantic Inference:** Use transitive logic to map anatomical relationships (e.g., Infection in the *Incus* → Infection in the *Temporal Bone*).
4.  **Standardization:** Classes are mapped to **SNOMED CT** identifiers for interoperability.

---

## 📂 Repository Structure

```text
/hospital-otology-ontology
│── diagram/
│   └── class-hierarchy.png
│
├── ontology/
│   └── clinical-ontology.ttl   # The complete, validated OWL/Turtle source code
│
├── output/                    # Evidence of validation
│   ├── evidence-inference.png  # Screenshot: Automatic Patient Classification
│   └── report-medication.png   # Screenshot: SPARQL Administrative Report
│
└── README.md                   # Project documentation
