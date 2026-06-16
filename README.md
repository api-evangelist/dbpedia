# DBpedia (dbpedia)

DBpedia is a community project that extracts structured data from Wikipedia and publishes it as Linked Open Data on the Web. It provides a SPARQL endpoint, a Lookup Service for entity resolution, a Spotlight API for text annotation, a Live endpoint for real-time Wikipedia data, and Linked Data access via HTTP content negotiation — forming a queryable cross-linked knowledge graph of Wikipedia-derived facts.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/dbpedia/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/dbpedia/refs/heads/main/apis.yml)

## Tags

- Linked Data
- Knowledge Graph
- SPARQL
- Semantic Web
- Wikipedia
- Open Data
- Entity Linking
- RDF
- Ontology

## Timestamps

- **Created:** 2026-06-13
- **Modified:** 2026-06-13

## APIs

### DBpedia SPARQL Endpoint

Public SPARQL 1.1 query endpoint backed by OpenLink Virtuoso over the DBpedia knowledge graph derived from Wikipedia. Supports up to 10,000 result rows, 120-second query timeout, and 100 requests/second per IP. Returns data in HTML, XML, JSON, Turtle, RDF/XML, N-Triples, CSV, and TSV. Loads the Databus Latest Core Collection for continuous updates.

- **Human URL:** [https://www.dbpedia.org/resources/sparql/](https://www.dbpedia.org/resources/sparql/)
- **Base URL:** `https://dbpedia.org/sparql`

#### Tags

- SPARQL
- Knowledge Graph
- RDF
- Wikipedia
- Linked Data
- Semantic Web

#### Properties

- [Documentation](https://www.dbpedia.org/resources/sparql/)
- [Terms of Service](https://www.dbpedia.org/resources/sparql/)

### DBpedia Lookup Service

REST API for entity retrieval and auto-complete over the DBpedia knowledge graph. Resolves plain-text keywords to DBpedia resource URIs. Supports keyword search (/api/search) and prefix/auto-complete search (/api/prefix). Query parameters include query, type (DBpedia ontology class filter), and maxResults. Responses available in XML (default) and JSON with result highlighting.

- **Human URL:** [https://www.dbpedia.org/resources/lookup/](https://www.dbpedia.org/resources/lookup/)
- **Base URL:** `https://lookup.dbpedia.org/api`

#### Tags

- Entity Lookup
- Auto-Complete
- Knowledge Graph
- REST
- Entity Resolution

#### Properties

- [Documentation](https://www.dbpedia.org/resources/lookup/)
- [Git Hub](https://github.com/dbpedia/dbpedia-lookup)

### DBpedia Spotlight

REST API for automatic annotation and entity linking of natural language text to DBpedia resources. Accepts text via HTTP GET or POST and returns mentions linked to DBpedia URIs. Supports multi-language entity spotting and disambiguation. Output formats include XML, JSON, Turtle, N-Triples, and RDF/XML. Can also be self-hosted via Docker.

- **Human URL:** [https://www.dbpedia.org/resources/spotlight/](https://www.dbpedia.org/resources/spotlight/)
- **Base URL:** `https://api.dbpedia-spotlight.org`

#### Tags

- Entity Linking
- Text Annotation
- NLP
- REST
- Knowledge Graph
- Named Entity Recognition

#### Properties

- [Documentation](https://www.dbpedia.org/resources/spotlight/)
- [Git Hub](https://github.com/dbpedia/dbpedia-spotlight-model)

### DBpedia Linked Data

HTTP Linked Data access to DBpedia resources via content negotiation. Dereference any DBpedia entity URI (http://dbpedia.org/resource/{EntityName}) using an Accept header to retrieve RDF descriptions in JSON-LD, Turtle, N3, RDF/XML, N-Triples, or HTML. Redirects via 303 See Other to format-specific document URIs (e.g. /data/Berlin.ttl). Language-specific chapters available (e.g. http://es.dbpedia.org/resource/).

- **Human URL:** [https://www.dbpedia.org/resources/linked-data/](https://www.dbpedia.org/resources/linked-data/)
- **Base URL:** `https://dbpedia.org/resource`

#### Tags

- Linked Data
- RDF
- Content Negotiation
- Semantic Web
- HTTP
- Knowledge Graph

#### Properties

- [Documentation](https://www.dbpedia.org/resources/linked-data/)

### DBpedia Live

Real-time SPARQL endpoint and Linked Data access over continuously updated DBpedia data derived from near-real-time Wikipedia edits. SPARQL endpoint at http://live.dbpedia.org/sparql. Provides 19 types of Wikipedia content including abstracts, images, person data, and external links. Processes approximately 105 Wikipedia page modifications per minute. Changesets available for download.

- **Human URL:** [https://www.dbpedia.org/resources/live/](https://www.dbpedia.org/resources/live/)
- **Base URL:** `https://live.dbpedia.org/sparql`

#### Tags

- Real-Time
- SPARQL
- Wikipedia
- Knowledge Graph
- Live Data
- RDF

#### Properties

- [Documentation](https://www.dbpedia.org/resources/live/)

### DBpedia Databus

Data cataloging, versioning, and publishing platform for DBpedia and community datasets. Exposes a SPARQL API for querying RDF metadata and a Search API for discovering published datasets. Data metadata is signed with X.509 certificates and WebID for provenance. Programmatic access via the Databus Client tool and HTTP API. Supports automated publishing pipelines.

- **Human URL:** [https://www.dbpedia.org/resources/databus/](https://www.dbpedia.org/resources/databus/)
- **Base URL:** `https://databus.dbpedia.org`

#### Tags

- Data Catalog
- Dataset Discovery
- SPARQL
- RDF
- Versioning
- Open Data

#### Properties

- [Documentation](https://dbpedia.gitbook.io/databus)
- [Git Hub](https://github.com/dbpedia/databus)

## Common Properties

- [Website](https://www.dbpedia.org/)
- [Documentation](https://www.dbpedia.org/resources/)
- [Git Hub](https://github.com/dbpedia)
- [Forum](https://forum.dbpedia.org/)
- [Blog](https://www.dbpedia.org/blog/)
- [Plans](plans/dbpedia-plans-pricing.yml)
- [Rate Limits](rate-limits/dbpedia-rate-limits.yml)
- [Fin Ops](finops/dbpedia-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
