# Changelog

All notable changes to the CE-RISE Circularity and End-of-Life Data Model will be documented in this file.

## [0.0.1] - 2025-12-12

### Added
- Initial project structure and repository setup from template: https://ce-rise-models.codeberg.page/template-data-model/
- Complete data model structure for Circularity and End-of-Life with 4 implementation stages:
  - **Stage 1: DesignForCircularity** - Design features enabling circular economy (modularity, materials, disassembly, durability)
  - **Stage 2: ProductPerformanceFactors** - Quantifiable performance metrics (resource efficiency, lifespan factors, circular capability)
  - **Stage 3: CircularityAssessments** - Generic assessment container supporting multiple methodologies with sub-scores
  - **Stage 4: EndOfLifeInformation** - Comprehensive EOL pathways (collection, recycling, CRM recovery, treatment options)
- External ontology imports using owl.filler pattern:
  - CHEBI for chemical entities and hazardous substances
  - ENVO for environmental concepts (waste, emissions, landfill)
  - Schema.org for instructions, lifetime, maintenance
  - QUDT for quantities and units
  - BFO for temporal/reliability concepts
  - ODP for design patterns
  - Dublin Core for metadata and provenance
- Unique SQL identifiers for all fields following `circ_[category]_[specific]` pattern
- Support for multiple assessments over time (repeatable/multivalued)
- Autonomous model design with interoperability potential
- No required fields maintaining flexibility
- Appropriate data types (float for percentages/metrics, string for descriptions, date for timestamps)
- Critical Raw Materials (CRM) recovery tracking
- Multi-valued material lists for comprehensive tracking
- Artifacts built and deployed to pages
