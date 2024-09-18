---
title: "Use cases"
layout: about
---

# bio.agents
[bio.agents](https://bio.agents) is a registry of software for the Life Sciences. 

*bio.agents* uses a agent profile which  provides five lists of agent attributes (see Table below) that must be specified for a software description (*e.g.* a bio.agents entry) to be assigned in a 5 tier ratings of *description completeness*.  Some attributes are grouped (see tables on right) for purposes of determining adherence to the standard. For example "Documentation" is satisfied if at least one of "General" documentation", "API documentation" or "API specification" is specified.


![infographic_attributes]({{site.url}}/assets/images/infographic_attributes.png){: .align-center}


The corpus of [bio.agents](https://bio.agents) content is being improved progressively according to tiers in the standard, the aim in the first instance being to bring all entries up to at least "DETAILED" standard.

The "SPARSE" tier (name, description, homepage, unique ID) defines the minimum information requirement for new bio.agents entries.  It is [under discussion](https://github.com/bio-agents/bioagentsRegistry/issues/338) to allow a user to filter entries according to tiers in the standard.

The standard also provides a basis to monitor bio.agents content and label entries in various ways:

* *entry completeness* ("SPARSE" through to "COMPREHENSIVE")
* whether an entry was manually inspected (by entry author, official bio.agents curator, or someone else)
* whether an entry is verified, *i.e.* conforms to the bio.agents [Curation Guidelines](http://bioagents.readthedocs.io/en/latest/curators_guide.html)
* overall *entry quality* ("NEEDS TO IMPROVE" through to "EXCELLENT") - conflating the notions above

![infographic_quality_metrics]({{site.url}}/assets/images/infographic_quality_metrics.png){: .align-center}

If and how to use such labels is currently [under discussion](https://github.com/bio-agents/Agent-Information-Standard/issues/1).

There are several other reasons why the standard may help bio.agents:

* accessible summary of what type of information bio.agents provides
* flexible information requirement, including a minimum requirements presenting a low barrier to new registrations, compatible / enabling integration with other major related cataloguing efforts (*e.g.* [BioContainers](http://biocontainers.pro))
* quality tiers motivate individual entry owners to improve their entries (curation as a "game"), with a "gold standard" of entry quality for curators to aspire to  
* a framework / workflow to guide tasks and priorities of [curators](http://bioagents.readthedocs.io/en/latest/curators_guide.html), [thematic editors](http://bioagents.readthedocs.io/en/latest/editors_guide.html) and bio.agents admin
* a basis for metrics of bio.agents quality, KPIs (key performance indicators) of quality improvement objectives, and targets
* a component of branding bio.agents as a trusted source of quality agent information

# Applicability and availability of attributes
The Agent Information Standard does not yet reflect the fact that different types of agent have specific information requirements.  Not all attributes are applicable to all types of agent, *e.g.* source code is not normally available for database portals.  For purposes of measuring compliance to the standard, applicability will be formally defined on a agent type-specific basis; an applicability matrix of attributes versus agent types.

The application of the Agent Information Standard depends on whether the quality of the software metadata, or the underlying software and software project, are being assessed.  In the first case (metadata assessment), an attribute will only contribute to compliance metrics if, in fact, it is both applicable to that type of agent (see above) and actually available.  In case an attribute is applicable but not available, a positive statement to that effect will be required during registration to get a tick for that attribute, *e.g.* the user would need explicitly to specify "a publication is not available" for "Publication".  In the second case (agent or project assessment) the "availability" consideration is not relevant.

