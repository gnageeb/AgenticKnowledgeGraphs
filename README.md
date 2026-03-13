# Pluralsight Agentic Knowledge Graphs - Demo Files Guide

> **Note:** This guide describes the structure and purpose of demo files. For detailed course content and explanations, refer to the official Pluralsight course [here](https://app.pluralsight.com/ilx/video-courses/agentic-knowledge-graphs) .

---

## Overview

The Agentic Knowledge Graphs course includes practical demonstrations across three modules that illustrate key concepts through working code examples and implementations.

---


## Module 2 Demos: Building & Integration

### Demo 2: Updating the Graph Without Duplicates

**Purpose:** Shows the practical challenges and solutions for incremental graph updates while maintaining data quality.

**Demo Components:**

#### Build & Update Phase
- Build a baseline knowledge graph
- Add new data through triplets
- Observe effects of naive updates

#### Fix & Verify Phase
- Canonicalize entity names
- Apply deduplication strategies
- Verify graph integrity with visualization

**Key Learning:** Demonstrates the importance of entity normalization and merge operations for maintaining clean, accurate graphs.

**Expected Outcomes:**
- A stable graph without duplicate nodes
- Properly unified evidence across related entities
- Reusable nodes across multiple data sources

---

### Demo 3: Building a Simple Knowledge Graph Pipeline in Neo4j

**Purpose:** Provides a complete end-to-end walkthrough of setting up a graph database and connecting it with agent reasoning.

**Demo Scope:**
- Neo4j installation and configuration
- Ingesting structured triplets into the graph
- Constructing basic queries
- Demonstrating agent reasoning over the graph

**Expected Setup:**
- Working Neo4j instance with sample data
- Populated graph with nodes and relationships
- Executable queries for retrieval

**Real-World Application:** Shows how support ticket data flows from extraction → storage → querying → agent response.

---

## Module 3 Demos: Frameworks & Production

### Demo Context: Production-Ready Implementation

The final module builds on previous demos by discussing production considerations:
- Scaling the demo setup
- Adding governance and monitoring
- Implementing query optimization
- Managing schema evolution

**No standalone demo in Module 3**, but the concepts build directly from Module 2's Neo4j example.

---

## Demo Data: The Support Ticket Case Study

All demos use a consistent dataset based on customer support tickets with:

**Sample Entities:**
- Customers
- Products (laptops, devices, software)
- Issues (overheating, battery drain, crashes)
- Resolutions (patches, updates, documentation)

**Sample Relationships:**
- Customer REPORTS Issue
- Issue AFFECTS Product
- Issue CAUSED_BY Root Cause
- Issue RESOLVED_BY Resolution

**Why This Case Study:** The support ticket domain is realistic, relatable, and demonstrates core agentic knowledge graph patterns applicable to many industries.

---

## Demo Technology Stack

| Component | Technology | Purpose |
|-----------|-----------|---------|
| **Graph Database** | Neo4j | Primary storage and querying |
| **Query Language** | Cypher | Graph pattern matching and retrieval |
| **Agent Integration** | Python (LLM calls) | Connecting LLM reasoning to graph queries |
| **Data Format** | Structured Triplets | Entities, relationships, properties |

---

## Learning Path Through Demos

```
Module 1: Understand the Problem
  ↓
Module 2: Learn Implementation Patterns
  ↓
Module 2 Demo 1: Handle Duplicates
  (Update → Deduplicate → Merge)
  ↓
Module 2 Demo 2: Build Production Graph
  (Storage → Query → Agent Integration)
  ↓
Module 3: Production Considerations
  (Scaling, Governance, Optimization)
```

---

## What Each Demo Teaches

### Demo 1: Extracting Entities & Relationships
- **Problem Solved:** How to convert unstructured text into graph-ready data
- **Technical Skills:** NLP extraction, entity typing, relationship discovery
- **Practical Takeaway:** Automation of data preparation for graphs

### Demo 2: Deduplication & Merge Operations
- **Problem Solved:** Maintaining data quality during incremental updates
- **Technical Skills:** Entity canonicalization, MERGE operations, graph validation
- **Practical Takeaway:** Graphs stay clean and evidence stays unified as data grows

### Demo 3: Neo4j Pipeline
- **Problem Solved:** End-to-end graph setup and agent integration
- **Technical Skills:** Database setup, query writing, tool integration
- **Practical Takeaway:** How to make graphs actionable with agents

---

## Prerequisites for Running Demos

To work through the demos, you typically need:

- Python 3.8+ environment
- Neo4j Community or Enterprise edition
- Python libraries: Neo4j driver, LLM SDK, data processing (pandas, etc.)
- Understanding of basic graph concepts
- Access to sample dataset (provided in course)

---

## Next Steps After Demos

Following the demonstrations, the course covers:
- **Testing** your graph implementation
- **Optimizing** queries for performance
- **Scaling** to larger datasets
- **Maintaining** schema consistency
- **Monitoring** graph health

---

## Summary

The demos progress from foundational concepts (extraction) through practical implementation (building & updating) to production considerations (scaling & governance). Each builds on previous knowledge while introducing new challenges and solutions.

For full details on implementation, best practices, and theory, refer to the complete Pluralsight course materials.

---

**Course:** Agentic Knowledge Graphs (Pluralsight)
**Platform:** Pluralsight Learning Platform
