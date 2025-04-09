---
title: Review group name
nav_order: 5
---

# Review group name (essential 🟢)

### Description/Meaning

The name of the community or organisation that is submitting the review to metadata services and responsible for updating the metadata records. Not the authors of the review.

### **🤖**Examples

*code example of fields the metadata can be mapped to and how to retrieve an example*

#### Crossref

##### **Deposit**

```
<institution>Review group name</institution>
```

See [Peer reviews markup guide](https://www.crossref.org/documentation/schema-library/markup-guide-record-types/peer-reviews/#00077)

##### **Retrieval**

```
{"institution":[
{
"name":"Review Commons"
}
]
```

#### DataCite

##### **Deposit** **Retrieval**

```
<publisher xml:lang="en" publisherIdentifier="https://ror.org/04z8jg394" publisherIdentifierScheme="ROR" schemeURI="https://ror.org/">Helmholtz Centre Potsdam - GFZ German Research Centre for Geosciences</publisher>
Definition: The name of the entity that holds, archives, publishes, prints, distributes, releases, issues, or produces the resource. This property will be used to formulate the citation, so consider the prominence of the role. 
```

#### DocMaps

A field "name" on the input of the first step (see [full examples](https://data-hub-api.elifesciences.org/enhanced-preprints/docmaps/v2/by-publisher/elife/get-by-manuscript-id?manuscript_id=86824)).

```
{
  ...
  "steps": {    "_:b0": {      "inputs": [{
        "publisher": "name":,
        ...
     }]
    }
  }
}
```

### 🙏Who is currently depositing/retrieving this metadata and can help others? 

| Organisation and contact email | Workflow example |
| :---- | :---- |
| eLife Sciences Publications, | [6\. Publish-Review-Curate platform](https://osf.io/preprints/metaarxiv/yu4sm_v1) |
| PREreview | [4\. Preprint review platform using a repository](https://osf.io/preprints/metaarxiv/yu4sm_v1) |
| Sciety |  |
| Review Commons |  |
| F1000, michael.evans@f1000.com | [5\. Open Research platform](https://osf.io/preprints/metaarxiv/yu4sm_v1) |

### 💪Actions/updates from the community 

The comments section provides a way for the preprint review community to discuss approaches to implementation of the metadata. Here you can show how you are depositing and using the metadata and provide updates.

{% include giscus.html %}