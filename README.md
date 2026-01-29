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

```
```markdown
### Logic Flow Diagram
![Safety Logic Diagram](https://mermaid.ink/img/pako:eNp1U9tu2zAM_RXBzylQ-wF7G7A1WIDsMGxD1wV7cCJbM2RJo-S4QZD_PpScxGl7CzzEkYfnkFQqaY0S0uD9r0Zz98L04yvTy2W72ez1er-VfC_57Xq9lQ_bteQ3GyluN_tCOh5oQYVn16fK4D9d3hV8d-sP09-gN7_I7uXjY6nZ6_fS8U8pP-72hXw8Svl4LOUO_y6l3En5sC8s4D9cO-zJgQ9F81N4V_C36538uHuQj4f97u4Jp-7X58K7gu_Q1i_k9j6Q9N4V_P36Q3b3q3R0e_gO4_h1I_nxd9ntHy3g_4Xq8-W5tPbC9MMJd3a4F6b_Bq390oI-9A9-mH54V_D3j7v8D7_8cZf74S77w62s9690-IflXcH333f5H375_S73w132h1tp9R9N-I1l-xXG6H1Fp2f-cO6_sYxftoRj0aT0r6T8J1r6t3_b8q4w_XDCp_QfTfiM5e-3zN-u2690wqeP9i_vCr7_usv_8Muvd7kf7rI_3Eqr_2jCb6z7rxAm8xL4I9A5SIm_Ah0w1sAIsACWQAcsgB7YAHtgDwyBETAABkAPGAKjYAyMgTEwAaZAD0yBGTAFZsAcmANzYAFMgQUwBxbAApgDS2AJLIEesAR6wBJYASuACbACVoAJwASYA0yAGcAEWAArgBXAClgBrIA1wApYA2uADbABNgAbYAusgI2ADbAFNgI2wBbYClgB2wBbYAdggx2AHbADsAP2AENgD-wBhsAeYAjsAYbAHmAI7AGGwB5gCOwBhgADDAEGGAIMMAYwABhgDDDAGMAAYIAxgAHAAAdgAAwABjgAA2AAMMABGAADYAAMgAEwAAbAABgAA2AADAAGGAAMMAYwABjAAGCAA4ABDgAGOAAY4ABggAOAAQ4ABjgAGOAA4P8H_wF074iE)
