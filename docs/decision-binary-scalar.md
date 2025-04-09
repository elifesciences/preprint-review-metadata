---
title: Decision (Binary/Scalar)
nav_order: 7
---

# Decision (Binary/Scalar) (essential 🔴)

### Description/Meaning

This is an outcome of the peer review process. 

### **🤖**Examples

*code example of fields the metadata can be mapped to and how to retrieve an example*

#### Crossref

##### **Deposit**

```
<recommendation>major-revision</recommendation>
```

Allowed values: major-revision, minor-revision, reject, reject-with-resubmit, accept

##### **Retrieval**

```
"review": {
"type": "referee-report",
"recommendation": "major-revision"
},
```

Example [record](https://www.crossref.org/documentation/schema-library/markup-guide-record-types/peer-reviews/#00077) 

#### DataCite

##### **Deposit** **Retrieval**

```
Not currently supported
```

#### DocMaps

```
Not currently supported
```

### 🙏Who is currently depositing/retrieving this metadata and can help others? 

| Organisation and contact email | Workflow example |
| :---- | :---- |
|  |  |

### 💪Actions/updates from the community

The comments section provides a way for the preprint review community to discuss approaches to implementation of the metadata. Here you can show how you are depositing and using the metadata and provide updates.

{% include giscus.html %}

#### F1000

The full text XML of any preprint Peer Reviews are incorporated into the Full Text XML of the preprints they review. The reviews are included as \<sub-articles\> with an @article-type attribute value of "reviewer-report".

There are three decision statuses reviewers can assign their reports: 

* Approved  
* Approved with Reservations  
* Not Approved

Those decisions are published as part of the peer review text. They are also included in the XML in a \<custom-meta-group\>, for example:

| \<custom-meta\-group\>	\<custom-meta\>        	\<meta\-name\>recommendation\</meta\-name\>                \<meta\-value\>approve\</meta\-value\>        \</custom-meta\>\</custom-meta\-group\> |
| :---- |

The \<meta-value\> options are: "approve", "approve-with-reservations", "reject", which correspond to "Approved", "Approved with Reservations", "Not Approved" respectively.

The XML can be retrieved via the F1000 API, using a DOI search: [https://verixiv.org/extapi/article/xml?doi=10.12688/verixiv.77.3](https://verixiv.org/extapi/article/xml?doi=10.12688/verixiv.77.3).

In the future, F1000 would like to add information about pre-publication checks to the review metadata record, in particular around data availability, plagiarism, ethics, etc. This is important to ensure transparency of the peer review process but is not currently supported by existing schemas.

#### eLife

eLife controlled vocabulary terms are captured in JATS XML using \<kwd-group\>. These are captured at the \<sub-article\> level (i.e. in the eLife Assessment itself, rather than for the article). They are not currently exposed at Crossref or elsewhere as there are currently no appropriate fields to capture this content.

```
<kwd-group kwd-group-type="claim-importance">
<!-- Controlled vocabulary of importance values: Landmark; Fundamental; Important; Valuable; Useful -->
<!-- 0 or 1 term may be selected -->
    <kwd>Valuable</kwd>
</kwd-group>
<kwd-group kwd-group-type="evidence-strength">
<!-- Controlled vocabulary of strength values: Exceptional; Compelling; Convincing; Solid; Incomplete; Inadequate -->
<!-- Multiple terms may be selected -->
    <kwd>Compelling</kwd>
    <kwd>Incomplete</kwd>
</kwd-group>
```

eLife XML can be accessed at the following github repo: [https://github.com/elifesciences/elife-article-xml](https://github.com/elifesciences/elife-article-xml)    
(note that at time of writing Reviewed Preprint XML is not currently available, but we aim to change that in the future)

In addition these terms are available via the eLife API, but while publicly available, this is deliberately not publicly exposed. 