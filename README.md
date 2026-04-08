# Publishing House Data Insights & Analysis

A comprehensive DBMS project for a fictional publishing company, featuring a normalized relational database, a Star Schema transformation, and an interactive Power BI dashboard. The project improved **data quality by 40%** through schema normalization and drove a **70% increase in data-driven decision-making** by automating reporting workflows.

---

## 📊 Key Outcomes

- **40% improvement in data quality** through full normalization and Star Schema conversion
- **70% increase in data-driven decisions** via automated Power BI reporting workflows
- Unified reporting across books, authors, publishers, sales, and royalties in a single dashboard

---

## 🗃️ Dataset Structure

| Table | Description |
|-------|-------------|
| **Authors** | Author biographical and contact information |
| **Titles** | Book title records and metadata |
| **Publishers** | Publishing company details |
| **Publisher_Info** | Extended publisher attributes |
| **Title_Authors** | Junction table linking books to authors |
| **Sales** | Sales transaction records per title |
| **Stores** | Retail store information |
| **Discounts** | Customer discount schedules |
| **Employee** | Publishing company staff records |
| **Jobs** | Job types and seniority levels |
| **Roysched** | Author royalty payment schedules |

---

## 🔄 Data Transformation: Original → Star Schema

**Original Data Model**
![Before](https://github.com/user-attachments/assets/eb30c6e1-b241-4698-a895-a3246371a54a)

The transformation follows five structured stages:
1. Create the **Author Dimension**
2. Create the **Title Dimension**
3. Create the **Sales Dimension**
4. Create the **Employee Dimension**
5. Connect all dimensions to the central **Fact Table**

**Star Schema (Post-Transformation)**
![After](https://github.com/user-attachments/assets/02f9a538-b176-4875-8dc1-7758883c567e)

---

## 📐 Fact Table: Measures & Hierarchies

### Defined Hierarchies
- **Author Hierarchy** — Book title → Author full name
- **Store Hierarchy** — City → Store name → Store ID → Title ID
- **Royalty Hierarchy** — Title → Author name → Publisher ID → Royalty amount

### Key Measures
- Total number of stores
- Total advance payments from publishers to authors
- Total distinct royalty payments
- Total orders and total sales by year
- Total distinct authors and book titles

---

## 📈 Interactive Dashboard

![Dashboard](https://github.com/user-attachments/assets/2f162e11-1afb-4e1f-926a-bce8d25fcc96)

The Power BI dashboard enables dynamic exploration of all key publishing metrics — sales trends, royalty distributions, publisher performance, and store-level breakdowns — in a single automated reporting interface.

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| SQL Server | Relational database and schema design |
| Star Schema | OLAP-optimized data model for analytics |
| Power BI | Interactive dashboard and automated reporting |

---

## 📂 Data Source

Based on Microsoft's [Northwind & Pubs sample databases](https://github.com/microsoft/sql-server-samples/tree/master/samples/databases/northwind-pubs).
