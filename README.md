# Schemalog — Structured Semantic Schemas for AI Systems

A framework for building machine-readable business schemas across multiple domains.

## What This Is

Most business data exists in formats optimized for human reading (web pages, PDFs, spreadsheets) or proprietary database storage. AI systems, search engines, and automated workflows struggle to extract structured meaning from these formats at scale.

Schemalog provides domain-specific schema implementations that bridge this gap — making business logic machine-readable while remaining human-comprehensible. Each implementation follows Schema.org conventions where applicable and extends them where domain-specific semantics require it.

## Philosophy

Structured data is infrastructure, not decoration. When business knowledge is locked in unstructured text and proprietary systems, AI models can't learn from it, search engines can't index it properly, and automated workflows can't act on it.

Schemalog treats schemas as **first-class artifacts** — not just metadata added after the fact, but the foundational structure that enables:

- **AI training and fine-tuning** on real-world business data
- **Semantic interoperability** between systems that were never designed to talk to each other
- **Automated reasoning** over business logic that currently requires human interpretation
- **Search engine understanding** that goes beyond keyword matching

## Domain Implementations

Each Schemalog project tackles a specific business domain where structured schemas unlock significant value:

### 🔮 [Codex — Tarot Reading Schema](https://github.com/tarotschema)
Structured semantic representation of tarot spreads, card meanings, and reading logic. Designed to enable AI-powered tarot interpretation systems that understand symbolic relationships rather than just text patterns.

**Status:** Spreads complete. Deck schemas in progress.  
**Use Case:** AI tarot readers, symbolic system training data, divination content automation.

---

### ☕ [Omni — Consumer Product Schema](https://github.com/schemalog/omni)
Product catalog schema that integrates marketplace reviews (Lazada, Shopee) with Schema.org Product markup for SEO and AI training.

**Status:** Production stable. Deployed at Waking Cup (wakingcup.com).  
**Proven Impact:** 110% sales increase on Lazada in 6 months post-implementation.  
**Use Case:** E-commerce review aggregation, marketplace sync, product recommendation models.

---

### 🏝️ [Apex — Tour & Activity Schema](https://github.com/schemalog/apex)
Structured schema for tour operators covering itineraries, bookings, reviews, and customer engagement workflows. Designed for the Southeast Asian tour market.

**Status:** Partial deployment. Review funnel in production testing at Tour Hub Asia (tourhubasia.com).  
**Use Case:** Automated review collection, post-tour content generation, tour recommendation engines.

---

### 🏠 [Nexus — Real Estate Schema](https://github.com/schemalog/nexus)
Property listing schema for Thai real estate market. Extends Schema.org Place and Offer with Thailand-specific attributes: BTS/MRT proximity, flood risk zones, NPA (bank repo) status, FSBO classification.

**Status:** In development. Target deployment Q3 2026 at Sawasdee Realty (sawasdeerealty.com).  
**Use Case:** Lead scoring pipelines, environmental risk disclosure, agent CRM systems.

---

## Technical Approach

Each domain schema is implemented with:

- **JSON-LD** for web publication and linked data interoperability
- **Python data classes** for programmatic access and validation
- **Schema.org vocabulary** as base standard, extended where necessary
- **Real-world validation** through deployment in active businesses
- **Documentation** explaining design decisions and usage patterns

## Why Multiple Domains?

Building schemas across diverse domains (tarot, e-commerce, tours, real estate) demonstrates that the Schemalog approach is **domain-agnostic**. The same structured thinking that makes tarot readings machine-interpretable also makes product catalogs, tour itineraries, and property listings legible to AI systems.

This breadth matters because AI engineers increasingly work across domains rather than specializing in a single vertical. The ability to extract structure from messy real-world data regardless of domain is a transferable skill.

## Real-World Impact

Schemalog schemas are not academic exercises. Each one is deployed in production businesses:

| Schema | Business | Measurable Outcome |
|--------|----------|-------------------|
| Omni | Waking Cup | +110% Lazada sales (6 months) |
| Apex | Tour Hub Asia | 40-60% review request engagement (testing) |
| Codex | Tarotsmith | 16 years production (2009-2025) |
| Nexus | Sawasdee Realty | In development |

## Use Cases for AI and Automation

### 1. Training Data for Domain-Specific Models
Structured schemas provide clean training data for fine-tuning models on specific domains. A product recommendation model trained on Omni-structured data understands product relationships, review sentiment, and marketplace dynamics in ways that raw text cannot convey.

### 2. RAG Systems and Knowledge Graphs
Schemas enable retrieval-augmented generation systems to query business knowledge semantically rather than through keyword matching. A tour operator chatbot powered by Apex schema understands itinerary logistics, availability constraints, and customer preferences.

### 3. Automated Workflow Integration
Machine-readable schemas allow systems that were never designed to integrate to share structured data. An e-commerce store using Omni schema can automatically sync with marketplaces, social media, and AI recommendation engines without custom API development for each platform.

### 4. Search Engine Optimization
Schema.org-compliant structured data improves search visibility through rich snippets, knowledge panels, and enhanced result displays. Proper schema markup is infrastructure for discoverability.

### 5. Semantic Interoperability
Organizations using compatible schemas can exchange data without custom integration work. A tour operator using Apex schema can share itinerary data with booking platforms, review aggregators, and customer relationship systems that understand the same semantic structure.

## Roadmap

### Short Term (Q1-Q2 2025)
- Complete Codex deck schemas
- Deploy Nexus at Sawasdee Realty
- Publish Omni and Apex as stable releases with full documentation
- Add schema validation tooling

### Medium Term (Q3-Q4 2025)
- Document AI integration patterns and example implementations
- Build reference implementations for common use cases (RAG systems, recommendation engines)
- Expand to additional domains based on operational need

### Long Term (2026+)
- Establish Schemalog as a recognized framework for domain-specific schema development
- Community contributions and collaborative schema evolution
- Cross-domain integration patterns (e.g., real estate + tour bookings for relocation services)

## Contributing

Schemalog schemas are extracted from real businesses I operate. This hands-on approach ensures schemas solve actual problems rather than theoretical ones.

Contributions are welcome once initial implementations stabilize. The goal is not to build schemas by committee, but to build them through operational deployment and then refine them through community feedback.

If you're building in one of these domains and Schemalog schemas would be useful, reach out. Collaboration is more valuable than isolated development.

## Design Principles

1. **Real-world first** — Schemas emerge from operational deployment, not abstraction
2. **AI-native** — Optimized for machine interpretation, not just human reading
3. **Interoperable** — Schema.org compatible where applicable, cleanly extended where necessary
4. **Documented** — Design decisions explained, not just data structures published
5. **Validated** — Every schema field exists because it solved a real problem in production

## Why This Matters

The gap between "data exists" and "data is usable by AI systems" is the defining constraint of the current era. Structured schemas are the bridge. They're not glamorous — they're infrastructure. But infrastructure is what enables everything else.

Schemalog is an attempt to build that infrastructure publicly, domain by domain, validated through real-world deployment.

## Technical Stack

- **Python** for schema implementation and validation
- **JSON-LD** for linked data publication
- **Schema.org** as vocabulary foundation
- **Pydantic** for Python data class generation (where applicable)
- **GitHub** for version control and collaboration

## License

MIT License — free to use, extend, and embed in commercial or open-source projects.

## Related Work

- [Schema.org](https://schema.org) — Foundational vocabulary for structured data
- [JSON-LD](https://json-ld.org) — JSON-based linked data format
- [Google Structured Data Guidelines](https://developers.google.com/search/docs/appearance/structured-data/intro-structured-data) — SEO application of schema markup

## Contact

For questions about implementation, collaboration, or commercial use: [contact@schemalog.com]

---

**Built with real businesses. Deployed in production. Validated by outcomes.**
