---
title: Review date
nav_order: 6
---

# Review date (essential 🟡)

### Description/Meaning

The date that the review was first published.

### **🤖**Examples

*code example of fields the metadata can be mapped to and how to retrieve an example*

#### Crossref

##### **Deposit**

```
<publication_date media_type='online'>
<month>11</month>
<day>18</day>
<year>2024</year>
</publication_date>
```

##### **Retrieval**

```
"published":{
"date-parts":[
[2024,11,18]
]
}
```

Example [record](https://www.crossref.org/documentation/schema-library/markup-guide-record-types/peer-reviews/#00077) 

#### DataCite

##### **Deposit** **Retrieval**

```
date / dateType [issued]
<dates>
    <date dateType="Issued">2022-08-01</date>
</dates>
```

#### DocMaps

See [full example](https://data-hub-api.elifesciences.org/enhanced-preprints/docmaps/v2/by-publisher/elife/get-by-manuscript-id?manuscript_id=86824).

```
{
  ...
  "steps": {
    "_:b1": {
      "outputs": [{
        "published": "2023-05-02T10:06:42.107967+00:00",
      }]
    }
  }
 }
```

### 🙏Who is currently depositing/retrieving this metadata and can help others? 

| Organisation and contact email | Workflow example |
| :---- | :---- |
| Copernicus GmbH |  |
| eLife Sciences Publications, | [6\. Publish-Review-Curate platform](https://osf.io/preprints/metaarxiv/yu4sm_v1) |
| Qeios | [1\. Preprint server with an integrated review option](https://osf.io/preprints/metaarxiv/yu4sm_v1) |
| Microbiology Society | [5\. Open Research platform](https://osf.io/preprints/metaarxiv/yu4sm_v1) |
| Review Commons |  |
| ScienceOpen | [1\. Preprint server with an integrated review option](https://osf.io/preprints/metaarxiv/yu4sm_v1) |
| RR/ID |  |
| Peer Community In | [3\. Preprint review platform registering DOIs](https://osf.io/preprints/metaarxiv/yu4sm_v1) |

### 💪Actions/updates from the community 