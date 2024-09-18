---
title: "Agent attributes"
layout: about
---

Agent attribute that may be defined using [bioagentsSchema](https://github.com/bio-agents/bioagentsschema) are summarised below, organised into tables for convenience.

Column descriptions:

* **Attribute** - short attribute name
* **Description** - concise human-readable description of the attribute 
* **Format** - data type of the attribute as defined in bioagentsSchema
* **bioagentsSchema** - link to description of bioagentsSchema element corresponding to the attribute
* **agentInfoProfileSchema** - attribute name used in [agentInfoProfileSchema]()
* **Guideline** - link to the [Curators Guide](https://bioagents.readthedocs.io/en/latest/curators_guide.html) giving guidelines on how to curate the attribute in [bio.agents](https://bio.agents)

# General attributes


Attribute | Description | Format | bioagentsSchema | agentInfoProfileSchema | Guideline
--------- | ----------- | ------ | -------------- | --------------------- | ---------  
**Name** | Canonical software name assigned by the software developer or service provider | Text | [``<name>``](http://bio-agents.github.io/bioagentsSchema/#Link1D) | name | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#name-agent)
**Description** | Short and concise textual description of the software function | Text | [``<description>``](http://bio-agents.github.io/bioagentsSchema/#Link1E) | description | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#description)
**Homepage** | Homepage of the software, or some URL that best serves this purpose | URL | [``<homepage>``](http://bio-agents.github.io/bioagentsSchema/#Link1F) | homepage | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#homepage)
**bio.agents ID** | Unique ID (case insensitive) of the agent that is assigned upon registration of the software in bio.agents, normally identical to agent name. | Text (URL-safe version of agent name) | [``<bioagentsID>``](http://bio-agents.github.io/bioagentsSchema/#Link20) | bioagentsID | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#summary-bioagentsid)
**bio.agents CURIE** | bio.agents CURIE (compact URI) based on the bio.agents agent ID. | Text | [``<bioagentsCURIE>``](http://bio-agents.github.io/bioagentsSchema/#Link21) | bioagentsCURIE | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#summary-bioagentscurie)
**version** | Version information (typically a version number) of the software. | Text | [``<version>``](http://bio-agents.github.io/bioagentsSchema/#Link22) | version | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#version-agent)
**otherID** | A unique identifier of the software, typically assigned by an ID-assignment authority other than bio.agents. |  Text | [``<otherID>``](http://bio-agents.github.io/bioagentsSchema/#Link23) | otherID | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#other-ids)
**Agent type** | The type of application software: a discrete software entity can have more than one type. | [enum](http://bioagentsschema.readthedocs.io/en/latest/controlled_vocabularies.html#agent-type) (from bioagentsSchema) | [``<agentType>``](http://bio-agents.github.io/bioagentsSchema/#Link39) | agentType | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#agent-type)



# Scientific attributes

Attribute | Description | Format | bioagentsSchema | agentInfoProfileSchema | Guideline
--------- | ----------- | ------ | -------------- | --------------------- | ---------  
**Scientific topics** | General scientific domain the software serves or other general category, *e.g.* 'Proteomics' | Term and / or URI of [EDAM Topic](http://edamontology.org/topic_0004) concept(s) | [``<topic>``](http://bio-agents.github.io/bioagentsSchema/#Link3A) | topic | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#topic)
**Scientific operations** | The basic operation(s) performed by the software, *e.g.* 'Multiple sequence alignment' | Term and / or URI of [EDAM Operation](http://edamontology.org/operation_0004) concept(s) | [``<function><operation>``](http://bio-agents.github.io/bioagentsSchema/#Link27) | operation | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#operation)
**Type of input data** | Type of primary input data (if any), *e.g.* 'Protein sequences' | Term and / or URI of [EDAM Data](http://edamontology.org/data_0006) concept(s) | [``<function><input><data>``](http://bio-agents.github.io/bioagentsSchema/#Link18) | inputData | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#data-type-input-and-output-data)
**Type of output data** | Type of primary output data (if any), *e.g.* 'Sequence alignment' | Term and / or URI of [EDAM Data](http://edamontology.org/data_0006) concept(s) | [``<function><input>/<output><data>``](http://bio-agents.github.io/bioagentsSchema/#Link18) | outputData | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#data-type-input-and-output-data)
**Supported input data formats** | Allowed format(s) of primary inputs, *e.g.* 'FASTA' | Term and / or URI of [EDAM Format](http://edamontology.org/format_1915) concept(s) | [``<function><input><format>``](http://bio-agents.github.io/bioagentsSchema/#Link18) | inputFormat | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#data-format-input-and-output-data)
**Supported output data formats** | Allowed format(s) of primary outputs, *e.g.* 'Clustal' | Term and / or URI of [EDAM Format](http://edamontology.org/format_1915) concept(s) | [``<function><input>/<output><format>``](http://bio-agents.github.io/bioagentsSchema/#Link18) | outputFormat | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#data-format-input-and-output-data)
**Function note** | Concise comment about a agent function, if not apparent from the software description and EDAM annotations. | Text| [``<function><note>``](http://bio-agents.github.io/bioagentsSchema/#Link2A) | functionNote | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#note-function)
**Function command** | Relevant command, command-line fragment or option for executing this function / running the agent in this mode. | Text| [``<function><note>``](http://bio-agents.github.io/bioagentsSchema/#Link2B) | functionCmd | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#command)



# Technical attributes

Attribute | Description | Format | bioagentsSchema | agentInfoProfileSchema | Guideline
--------- | ----------- | ------ | -------------- | --------------------- | ---------  
**Operating system** | The operating system supported by a downloadable software package. | [enum](http://bioagentsschema.readthedocs.io/en/latest/controlled_vocabularies.html#operating-system) (from bioagentsSchema) | [``<labels><OperatingSystem>``](http://bio-agents.github.io/bioagentsSchema/#Link3B) | operatingSystem | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#operating-system)
**Language** | Name of programming language the software source code was written in, *e.g.* 'C'. | [enum](http://bioagentsschema.readthedocs.io/en/latest/controlled_vocabularies.html#programming-language) (from bioagentsSchema) | [``<language>``](http://bio-agents.github.io/bioagentsSchema/#Link3C) | language | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#programming-language)
**License** | Software or data usage license | [enum](http://bioagentsschema.readthedocs.io/en/latest/controlled_vocabularies.html#license) (from bioagentsSchema) | [``<labels><license>``](http://bio-agents.github.io/bioagentsSchema/#Link3D) | license | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#license)
**Collection** | Tag for a collection that the software has been assigned to within bio.agents. | Text | [``<labels><collectionID>``](http://bio-agents.github.io/bioagentsSchema/#Link3E) | collectionID | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#collection)
**Maturity** | How mature the software product is. | [enum](http://bioagentsschema.readthedocs.io/en/latest/controlled_vocabularies.html#maturity) (from bioagentsSchema) | [``<labels><maturity>``](http://bio-agents.github.io/bioagentsSchema/#Link3F) | maturity | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#maturity)
**Cost** | Monetary cost of acquiring the software. | [enum](http://bioagentsschema.readthedocs.io/en/latest/controlled_vocabularies.html#cost) (from bioagentsSchema) | [``<labels><Cost>``](http://bio-agents.github.io/bioagentsSchema/#Link40) | cost | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#cost)
**Accessibility** | Whether an online service is freely available for use. | [enum](http://bioagentsschema.readthedocs.io/en/latest/controlled_vocabularies.html#accessibility) (from bioagentsSchema) | [``<labels><Accessibility>``](http://bio-agents.github.io/bioagentsSchema/#Link41) | accessibility | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#accessibility)


# Link attributes

Attribute | Description | Format | bioagentsSchema | agentInfoProfileSchema | Guideline
--------- | ----------- | ------ | -------------- | --------------------- | ---------  
**Discussion forum** | Online forum for user discussions about the software. | URL | [``<link><type>Discussion forum</type>``]() | discussionForum | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#link-group)
**Helpdesk** | Helpdesk providing support in using the software. | URL | [``<link><type>Helpdesk</type>``]() | helpdesk | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#link-group)
**Issue tracker** | Link to tracker for software issues, bug reports, feature requests etc. | URL | [``<link><type>Issue tracker</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1A) | issueTracker | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#link-group)
**Mailing list** | Link to mailing list for software announcements, discussions, support etc. | URL | [``<link><type>Mailing list</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1A) | mailingList | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#link-group)
**Mirror** | Mirror of an (identical) online service. | URL | [``<link><type>Mirror</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1A) | mirror | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#link-group)
**Software catalogue** | Some registry, catalogue etc. other than bio.agents where the agent is also described. | URL | [``<link><type>Software catalogue</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1A) | softwareCatalogue | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#link-group)
**Repository** | A place where source code, data and other files can be retrieved from, typically via platforms like GitHub which provide version control and other features, or something simpler, e.g. an FTP site. | URL | [``<link><type>Repository</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1A) | repository | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#link-group)
**Social media** | A website used by the software community including social networking sites, discussion and support fora, WIKIs etc. | URL | [``<link><type>Social media</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1A) | socialMedia | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#link-group)
**Service** | An online service (other than Galaxy) that provides access (an interface) to the software. | URL | [``<link><type>Service</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1A) | service | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#link-group)
**Galaxy service** | An online service providing the agent through the Galaxy platform. | URL | [``<link><type>Galaxy service</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1A) | galaxyService | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#link-group)
**Technical monitoring** | Information about the technical status of a agent. | URL | [``<link><type>Technical monitoring</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1A) | technicalMonitoring | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#link-group)
**Misc link** | Other type of link for software - the default if a more specific type is not available. | URL | [``<link><type>Other</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1A) | linkOther | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#link-group)


# Download attributes

Attribute | Description | Format | bioagentsSchema | agentInfoProfileSchema | Guideline
--------- | ----------- | ------ | -------------- | --------------------- | ---------  
**API specification** | File providing an API specification for the software, e.g. Swagger/OpenAPI, WSDL or RAML file. | URL | [``<download><type>API specification</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1B) | apiSpecification | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#download-group)
**Biological data** | Biological data, or a web page on a database portal where such data may be downloaded. | URL | [``<download><type>Biological data</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1B) | biologicalData | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#download-group)
**Binaries** | Binaries for the software. | URL | [``<download><type>Binaries</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1B) | binaries | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#download-group)
**Command-line specification** | File providing a command line specification for the software. | URL | [``<download><type>Command-line specification</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1B) | commandlineSpecification | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#download-group)
**Container file** | Container file including the software. | URL | [``<download><type>Container file</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1B) | containerFile | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#download-group)
**Icon** | Icon of the software. | URL | [``<download><type>Icon</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1B) | icon | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#download-group)
**Screenshot** | Screenshot of the software. | URL | [``<download><type>Screenshot</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1B) | screenshot | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#download-group)
**Source code** | Software source code. | URL | [``<download><type>Source code</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1B) | sourceCode | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#documentation-group)
**Software package** | A software package; a bundle of files and information about those files, typically including source code and / or binaries. | URL | [``<download><type>Software package</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1B) | softwarePackage | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#documentation-group)
**Test data** | Data for testing the software is working correctly. | URL | [``<download><type>Test data</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1B) | testData | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#documentation-group)
**Test script** | Script used for testing testing whether the software is working correctly. | URL | [``<download><type>Test data</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1B) | testScript | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#documentation-group)
**Agent wrapper (CWL)** |  | URL | [``<download><type>Agent wrapper (CWL)</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1B) | agentWrapperCWL | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#download-group)
**Agent wrapper (galaxy)** | Galaxy agent configuration file (wrapper) for the software. | URL | [``<download><type>Agent wrapper (galaxy)</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1B) | agentWrapperGalaxy | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#download-group)
**Agent wrapper (taverna)** | Taverna configuration file for the software. | URL | [``<download><type>Agent wrapper (taverna)</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1B) | agentWrapperTaverna | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#download-group)
**Agent wrapper (other)** | Workbench configuration file (other than taverna, galaxy or CWL wrapper) for the software. | URL | [``<download><type>Agent wrapper (other)</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1B) | agentWrapperOther | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#download-group)
**VM image** | Virtual machine (VM) image for the software. | URL | [``<download><type>VM image</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1B) | vmImage | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#download-group)
**Downloads page** | Web page summarising general downloads available for the software. | URL | [``<download><type>Downloads page</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1B) | downloadsPage | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#download-group)
**Misc download** | Other type of download for software - the default if a more specific type is not available. | URL | [``<download><type>Other</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1B) | downloadsOther | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#download-group)


# Documentation attributes

Attribute | Description | Format | bioagentsSchema | agentInfoProfileSchema | Guideline
--------- | ----------- | ------ | -------------- | --------------------- | ---------  
**API documentation** | Human-readable API documentation. | URL | [``<documentation><type>API documentation</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1C) | apiDocumentation | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#documentation-group)
**Citation instructions** | Human-readable API documentation. | URL | [``<documentation><type>Citation instructions</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1C) | citationInstructions | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#documentation-group)
**Command-line options** | Information about the command-line interface to a agent. | URL | [``<documentation><type>Command-line options</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1C) | commandlineOptions | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#documentation-group)
**Contributions policy** | Information about policy for making contributions to the software project. | URL | [``<documentation><type>Contributions policy</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1C) | contributionsPolicy | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#documentation-group)
**General documentation** | General documentation | URL | [``<documentation><type>General</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1C) | generalDocumentation | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#documentation-group)
**FAQ** | Frequently Asked Questions (and answers) about the software. | URL | [``<documentation><type>FAQ</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1C) | faq | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#documentation-group)
**Governance** | Information about the software governance model. | URL | [``<documentation><type>Governance</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1C) | governance | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#documentation-group)
**Installation instructions** | Instructions how to install the software. | URL | [``<documentation><type>Installation instructions</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1C) | installationInstructions | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#documentation-group)
**User manual** | Information on how to use the software, tailored to the end-user. | URL | [``<documentation><type>User manual</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1C) | userManual | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#documentation-group)
**Release notes** | Notes about a software release or changes to the software; a change log. | URL | [``<documentation><type>Release notes</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1C) | releaseNotes | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#documentation-group)
**Terms of use** | Rules that one must agree to abide by in order to use a service. | URL | [``<documentation><type>Terms of use</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1C) | termsOfUse | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#documentation-group)
**Training material** | Online training material such as text on a Web page, a presentation, video, tutorial etc. | URL | [``<documentation><type>Training material</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1C) | trainingMaterial | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#documentation-group)
**Misc. documentation** | Some other type of documentation not listed in bioagentsSchema. | URL | [``<documentation><type>Other</type>``](http://bio-agents.github.io/bioagentsSchema/#Link1C) | documentationOther | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#documentation-group)


# Publication attributes

Attribute | Description | Format | bioagentsSchema | agentInfoProfileSchema | Guideline
--------- | ----------- | ------ | -------------- | --------------------- | ---------  
**Primary publication** | The principal publication about the agent itself; the article to cite when acknowledging use of the agent.  | DOI, PMID or PMCID | [``<publication>``](http://bio-agents.github.io/bioagentsSchema/#Link16) | publicationPrimary | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#publication-group)
**Method publication** | A publication describing a scientific method or algorithm implemented by the agent. | DOI, PMID or PMCID | [``<publication>``](http://bio-agents.github.io/bioagentsSchema/#Link16) | publicationMethod | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#publication-group)
**Usage publication** | A publication describing the application of the agent to scientific research, a particular task or dataset. | DOI, PMID or PMCID | [``<publication>``](http://bio-agents.github.io/bioagentsSchema/#Link16) | publicationUsage | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#publication-group)
**Benchmarking study publication** | A publication which assessed the performance of the agent. | DOI, PMID or PMCID | [``<publication>``](http://bio-agents.github.io/bioagentsSchema/#Link16) | publicationBenchmarkingStudy | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#publication-group)
**Review publication** | A publication where the agent was reviewed. | DOI, PMID or PMCID | [``<publication>``](http://bio-agents.github.io/bioagentsSchema/#Link16) | publicationReview | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#publication-group)


# Relation attributes

Attribute | Description | Format | bioagentsSchema | agentInfoProfileSchema | Guideline
--------- | ----------- | ------ | -------------- | --------------------- | ---------  
**isNewVersionOf** | The software is a new version of an existing software, typically providing new or improved functionality. | URL | [``<relation><type>isNewVersionOf</type>``](http://bio-agents.github.io/bioagentsSchema/#) | relationIsNewVersionOf | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#relation-group)
**hasNewVersion** | (inverse of above) | URL | [``<relation><type>hasNewVersion</type>``](http://bio-agents.github.io/bioagentsSchema/#) | relationHasNewVersion | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#relation-group)
**uses** | The software provides an interface to or in some other way uses the functions of other software under the hood, e.g. invoking a command-line agent or calling a Web API, Web service or SPARQL endpoint to perform its function. | URL | [``<relation><type>uses</type>``](http://bio-agents.github.io/bioagentsSchema/#) | relationUses | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#relation-group)
**usedBy** | (inverse of above) | URL | [``<relation><type>usedBy</type>``](http://bio-agents.github.io/bioagentsSchema/#) | relationUsedBy | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#relation-group)
**includes** | A workbench, agentkit or workflow includes some other, independently available, software. | URL | [``<relation><type>includes</type>``](http://bio-agents.github.io/bioagentsSchema/#) | relationIncludes | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#relation-group)
**includedIn** | (inverse of above) | URL | [``<relation><type>includedIn</type>``](http://bio-agents.github.io/bioagentsSchema/#) | relationIncludedIn | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#relation-group)


# Credit / contact attributes

Attribute | Description | Format | bioagentsSchema | agentInfoProfileSchema | Guideline
--------- | ----------- | ------ | -------------- | --------------------- | ---------  
**Primary contact** | The primary point of contact for the software. | Name, email, URL and/or ORCID iD | [``<credit><typeRole>Primary contact</typeRole>``](http://bio-agents.github.io/bioagentsSchema/#Link15) | creditprimaryContact | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#credit-group)
**Person credit** | Credit of an individual. | Name, email, URL and/or ORCID iD | [``<credit><typeRole>Primary contact</typeRole>``](http://bio-agents.github.io/bioagentsSchema/#Link15) | creditPerson | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#credit-group)
**Project credit** | Credit of a community software project not formally associated with any single institute. | Name, email, URL and/or ORCID iD | [``<credit><typeRole>Primary contact</typeRole>``](http://bio-agents.github.io/bioagentsSchema/#Link15) | creditProject | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#credit-group)
**Division credit** | Credit of or a formal part of an institutional organisation, e.g. a department, research group, team, etc. | Name, email, URL and/or ORCID iD | [``<credit><typeRole>Primary contact</typeRole>``](http://bio-agents.github.io/bioagentsSchema/#Link15) | creditDivision | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#credit-group)
**Institute credit** | Credit of an organisation such as a university, hospital, research institute, service center, unit etc. | Name, email, URL and/or ORCID iD | [``<credit><typeRole>Primary contact</typeRole>``](http://bio-agents.github.io/bioagentsSchema/#Link15) | creditInstitute | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#credit-group)
**Consortium credit** | Credit of an association of two or more institutes or other legal entities which have joined forces for some common purpose. Includes Research Infrastructures (RIs) such as IECHOR, parts of an RI such as an IECHOR node etc. | Name, email, URL and/or ORCID iD | [``<credit><typeRole>Primary contact</typeRole>``](http://bio-agents.github.io/bioagentsSchema/#Link15) | creditConsortium | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#credit-group)
**Funding agency credit** | Credit of a legal entity providing funding for development of the software or provision of an online service. | Name, email, URL and/or ORCID iD | [``<credit><typeRole>Primary contact</typeRole>``](http://bio-agents.github.io/bioagentsSchema/#Link15) | creditFundingAgency | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#credit-group)
**Developer credit** | Author of the original software source code. | Name, email, URL and/or ORCID iD | [``<credit><typeRole>Primary contact</typeRole>``](http://bio-agents.github.io/bioagentsSchema/#Link15) | creditDeveloper | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#credit-group)
**Maintainer credit** | Maintainer of a mature software providing packaging, patching, distribution etc. | Name, email, URL and/or ORCID iD | [``<credit><typeRole>Primary contact</typeRole>``](http://bio-agents.github.io/bioagentsSchema/#Link15) | creditMaintainer | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#credit-group)
**Provider credit** | Institutional provider of an online service. | Name, email, URL and/or ORCID iD | [``<credit><typeRole>Primary contact</typeRole>``](http://bio-agents.github.io/bioagentsSchema/#Link15) | creditProvider | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#credit-group)
**Documentor credit** | Author of software documentation including making edits to a bio.agents entry. | Name, email, URL and/or ORCID iD | [``<credit><typeRole>Primary contact</typeRole>``](http://bio-agents.github.io/bioagentsSchema/#Link15) | creditDocumentor | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#credit-group)
**Contributor credit** | Some other role in software production or service delivery including design, deployment, system administration, evaluation, testing, documentation, training, user support etc. | Name, email, URL and/or ORCID iD | [``<credit><typeRole>Primary contact</typeRole>``](http://bio-agents.github.io/bioagentsSchema/#Link15) | creditContributor | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#credit-group)
**Support credit** | Provider of support in using the software. | Name, email, URL and/or ORCID iD | [``<credit><typeRole>Primary contact</typeRole>``](http://bio-agents.github.io/bioagentsSchema/#Link15) | creditSupport | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#credit-group)
**IECHOR Node** | Name of the IECHOR Node that is credited. | [enum](http://bioagentsschema.readthedocs.io/en/latest/controlled_vocabularies.html#iechor-node) (from bioagentsSchema) | [``<iechorNode>``](http://bio-agents.github.io/bioagentsSchema/#Link43) | iechorNode | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#iechor-node)
**IECHOR Platform** | Name of the IECHOR Platform that is credited. | [enum](http://bioagentsschema.readthedocs.io/en/latest/controlled_vocabularies.html#iechor-platform) (from bioagentsSchema) | [``<iechorPlatform>``](http://bio-agents.github.io/bioagentsSchema/#Link43) | iechorPlatform | [link](http://bioagents.readthedocs.io/en/latest/curators_guide.html#iechor-platform)

