---
title: "Agent Information Standards"
layout: about
---

The **Agent Information Standards** are a stack of community-defined, open and integrated technologies, technical standards and guidelines:

![technology_stack]({{site.url}}/assets/images/technology_stack.png){: .align-center}

- **bioagentsCore** is a flat list of over 50 important scientific, technical and administrative **software attributes** that support cataloguing, discovery, use and interoperability of software. It will soon be made available in JSON format. {[repo](https://github.com/bio-agents/Agent-Information-Standards/blob/master/docs/agent_attributes.md/), [learn more]({{site.url}}/agent_attributes.html)}
- **EDAM** is an ontology of well-established, familiar concepts that are prevalent within bioinformatics and computational biology. It defines the **semantics** - a controlled vocabulary - to describe software functionality in terms of *operations*, types of input and output *data* and data *identifiers*, supported data *formats*, and common *topics*. {[repo](https://github.com/edamontology/edamontology), [readthedocs](https://edamontologydocs.readthedocs.io/en/latest/)}
- **bioagentsSchema** is a formalised XML schema (XSD) which defines a description model for bioinformatics software. It defines a **structure** and **syntax** for the 50 attributes listed in bioagentsCore. To enable concise information, standard identifiers are used where possible, including EDAM ontology for scientific aspects and internally-defined controlled vocabularies for technical aspects such as programming language and license. It defines the scope and content of the [bio.agents](https://bio.agents) registry of life science software. {[repo](https://github.com/bio-agents/bioagentsschema), [readthedocs](https://bioagentsschema.readthedocs.io/en/latest/)}
- **Agent information profiles** define lists of software attributes (from bioagentsCore) that can, should or must be specified for different types of agents within a set of agent descriptions. An individual profile - a JSON file conforming to agentInfoProfileSchema (JSON schema) - defines an **information requirements** that is tailored to an individual communities (national, scientific or technical).  Agent information profiles provide a practical **curation framework** and **metrics** for any corpus of agents. {[repo](http://github.com/bio-agents/agent-information-profile)}
- **Curation guidelines** describe conventions for *how* each attribute should be specified when describing a agent for registation in catalogues such as *bio.agents*.  These human-readable **user-friendly guidelines** provide information that goes beyond syntax and semantics provided by bioagentsSchema and EDAM. Beyond the general purpose [Curators Guide](https://bioagents.readthedocs.io/en/latest/curators_guide.html), a set of [tutorials](https://bioagents.readthedocs.io/en/latest/community_specific_guidelines.html) are being tailored to the specific requirements of national, scientific and technical community profiles. {[repo](https://github.com/bio-agents/bioagentsdocs)}
- **Software Best Practice** can be abstracted from the curation guidelines, for example, the [general recommendations](https://iechor-europe.org/about-us/commissioned-services/software-best-practices) being developed by [IECHOR](https://iechor-europe.org/) for the provision and documentation of software.


The standards support the broader *bio.agents* initative - fostered with support from IECHOR - which aspires to provide comprehensive and consistent information for all European bioinformatics resources:

* *Community curation of bioinformatics software and data resources* (2019), Briefings in Bioinformatics, [doi:10.1093/bib/bbz075](https://doi.org/10.1093/bib/bbz075)
* *The bio.agents registry of software agents and data resources for the life sciences* (2019), Genome Biology, [doi:10.1093/bioinformatics/btt113.](https://doi.org/10.1093/bioinformatics/btt113)
* *Agents and data services registry: a community effort to document bioinformatics resources* (2016), Nucleic Acids Research [doi:10.1093/nar/gkv1116](https://doi.org/10.1093/nar/gkv1116)

