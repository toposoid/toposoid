# Toposoid Community Edition
Toposoid is a knowledge base construction platform.
Toposoid has the following features.
* You can build a knowledge base just by entering sentences (Currently only supports Japanese and English).
* If you enter the text as it is, you can search the knowledge base and obtain inference results.
* This inferring program is designed so that developers can freely extend and replace it in their favorite programming language.

In this repository, it is published as Toposoid Community Edition. For more information -> https://toposoid.com/

## Outline Drawing
<img width="1760" alt="" src="https://user-images.githubusercontent.com/82787843/135850589-0df6b747-df02-435d-9992-ee1831fec916.png">

## Knowledge Base Image
<img width="1760" alt="" src="https://github.com/toposoid/toposoid/assets/82787843/a4ccaafd-cda0-4060-9e1f-8ea9a0d04dbf"/>

## Toposoid project dependencies
<img width="1760" alt="" src="https://github.com/user-attachments/assets/16faf7e6-2540-4d5c-a206-c2f29492971c"/>



| ProjectName                                                                                                                                  | Function                                                                                                                                                                                                  | Status |
|----------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------| - |
| toposoid                                                                                                                                     | Root project for all Toposoid projects                                                                                                                                                                    |
| [toposoid-component-dispatcher-web](https://github.com/toposoid/toposoid-component-dispatcher-web.git)                                       | This microservice integrates two major microservices. One is a microservice that analyzes the predicate argument structure of sentences, and the other is a microservice that makes logical inferences.   | [![Unit Test And Build Image Action](https://github.com/toposoid/toposoid-component-dispatcher-web/actions/workflows/action.yml/badge.svg)](https://github.com/toposoid/toposoid-component-dispatcher-web/actions/workflows/action.yml) |
| [toposoid-easy-search-web](https://github.com/toposoid/toposoid-easy-search-web)                                                             | This microservice provides a simple search API. Specifically, it supports text search and image search.                                                                                                   | [![Test And Build](https://github.com/toposoid/toposoid-easy-search-web/actions/workflows/action.yml/badge.svg)](https://github.com/toposoid/toposoid-easy-search-web/actions/workflows/action.yml) |
| [toposoid-knowledge-register-web](https://github.com/toposoid/toposoid-knowledge-register-web.git)                                           | This microservice provides the functionality for manual registration.                                                                      | [![Unit Test And Build Image Action](https://github.com/toposoid/toposoid-knowledge-register-web/actions/workflows/action.yml/badge.svg)](https://github.com/toposoid/toposoid-knowledge-register-web/actions/workflows/action.yml) |
| [toposoid-knowledge-register-subscriber](https://github.com/toposoid/toposoid-knowledge-register-subscriber.git)                                           |  This microservice provides the functionality for manual registration.   | [![Unit Test And Build Image Action](https://github.com/toposoid/toposoid-knowledge-register-subscriber/actions/workflows/action.yml/badge.svg)](https://github.com/toposoid/toposoid-knowledge-register-subscriber/actions/workflows/action.yml) 
| [toposoid-document-analysis-subscriber](https://github.com/toposoid/toposoid-document-analysis-subscriber.git)                                           |   This microservice provides the functionality to register from a document.  | [![Unit Test And Build Image Action](https://github.com/toposoid/toposoid-document-analysis-subscriber/actions/workflows/action.yml/badge.svg)](https://github.com/toposoid/toposoid-document-analysis-subscriber/actions/workflows/action.yml) 
| [toposoid-sat-solver-web](https://github.com/toposoid/toposoid-sat-solver-web)                                                               | This microservice provides solver functionality for Boolean satisfiability problems (SAT) or similar problems (Max-SAT etc.).                                                                             | [![Test And Build](https://github.com/toposoid/toposoid-sat-solver-web/actions/workflows/action.yml/badge.svg)](https://github.com/toposoid/toposoid-sat-solver-web/actions/workflows/action.yml) |
| [toposoid-sentence-parser-japanese-web](https://github.com/toposoid/toposoid-sentence-parser-japanese-web.git)                               | This Microservice analyzes the predicate argument structure of Japanese sentences and outputs the result in JSON.                                                                                         |[![Test And Build](https://github.com/toposoid/toposoid-sentence-parser-japanese-web/actions/workflows/action.yml/badge.svg)](https://github.com/toposoid/toposoid-sentence-parser-japanese-web/actions/workflows/action.yml)|  
| [toposoid-common-nlp-japanese-web](https://github.com/toposoid/toposoid-common-nlp-japanese-web.git)                                         | This Microservice provides an NLP function that handles Japanese and outputs the result in JSON.                                                                                                          |[![Test And Build](https://github.com/toposoid/toposoid-common-nlp-japanese-web/actions/workflows/action.yml/badge.svg)](https://github.com/toposoid/toposoid-common-nlp-japanese-web/actions/workflows/action.yml)|
| [toposoid-sentence-parser-english-web](https://github.com/toposoid/toposoid-sentence-parser-english-web.git)                                 | This Microservice analyzes dependency's structure of English sentences and outputs the result in JSON.                                                                                                    |[![Test And Build](https://github.com/toposoid/toposoid-sentence-parser-english-web/actions/workflows/action.yml/badge.svg)](https://github.com/toposoid/toposoid-sentence-parser-english-web/actions/workflows/action.yml)|
| [toposoid-common-nlp-english-web](https://github.com/toposoid/toposoid-common-nlp-english-web.git)                                           | This Microservice provides an NLP function that handles English and outputs the result in JSON.                                                                                                           |[![Test And Build](https://github.com/toposoid/toposoid-common-nlp-english-web/actions/workflows/action.yml/badge.svg)](https://github.com/toposoid/toposoid-common-nlp-english-web/actions/workflows/action.yml)|
| [toposoid-deduction-admin-web](https://github.com/toposoid/toposoid-deduction-admin-web.git)                                                 | This microservice provides the ability to manage multiple deductive inference logic to register, update microservices.                                                                                    |[![Unit Test And Build Image Action](https://github.com/toposoid/toposoid-deduction-admin-web/actions/workflows/action.yml/badge.svg)](https://github.com/toposoid/toposoid-deduction-admin-web/actions/workflows/action.yml)|  
| [toposoid-deduction-unit-exact-match-web](https://github.com/toposoid/toposoid-deduction-unit-exact-match-web.git)                           | This microservice provides the ability to determine if the text you enter matches the knowledge graph exactly. 　                                                                                          |[![Unit Test And Build Image Action](https://github.com/toposoid/toposoid-deduction-unit-exact-match-web/actions/workflows/action.yml/badge.svg)](https://github.com/toposoid/toposoid-deduction-unit-exact-match-web/actions/workflows/action.yml)| 
| [toposoid-deduction-unit-synonym-match-web](https://github.com/toposoid/toposoid-deduction-unit-synonym-match-web.git)                       | This microservice provides the ability to determine if the text you enter matches, provided that the knowledge graph and synonyms are equated.                                                            |[![Unit Test And Build Image Action](https://github.com/toposoid/toposoid-deduction-unit-synonym-match-web/actions/workflows/action.yml/badge.svg)](https://github.com/toposoid/toposoid-deduction-unit-synonym-match-web/actions/workflows/action.yml)|
| [toposoid-deduction-unit-sentence-vector-match-web](https://github.com/toposoid/toposoid-deduction-unit-sentence-vector-match-web)           | This microservice provides the ability to identify the input text as a distributed representation using the [Bert model](https://github.com/google-research/bert) and match it against the knowledge graph. |[![Test And Build](https://github.com/toposoid/toposoid-deduction-unit-sentence-vector-match-web/actions/workflows/action.yml/badge.svg)](https://github.com/toposoid/toposoid-deduction-unit-sentence-vector-match-web/actions/workflows/action.yml)|
| [toposoid-deduction-unit-image-vector-match-web](https://github.com/toposoid/toposoid-deduction-unit-image-vector-match-web)                 | This microservice makes inferences by matching images to a knowledge database.                                                                                                                            |[![Test And Build](https://github.com/toposoid/toposoid-deduction-unit-image-vector-match-web/actions/workflows/action.yml/badge.svg)](https://github.com/toposoid/toposoid-deduction-unit-image-vector-match-web/actions/workflows/action.yml)|
| [toposoid-deduction-unit-whole-sentence-image-match-web](https://github.com/toposoid/toposoid-deduction-unit-whole-sentence-image-match-web) | This microservice performs inference by comparing images with a knowledge database, and handles cases where images are linked to entire sentences.                                                        |[![Test And Build](https://github.com/toposoid/toposoid-deduction-unit-whole-sentence-image-match-web/actions/workflows/action.yml/badge.svg)](https://github.com/toposoid/toposoid-deduction-unit-whole-sentence-image-match-web/actions/workflows/action.yml)|
| [data-accessor-weaviate-web](https://github.com/toposoid/data-accessor-weaviate-web)                                                         | This microservice is a CUID wrapper for [Weaviate](https://github.com/weaviate/weaviate).                                                                                                                 |[![Test And Build](https://github.com/toposoid/data-accessor-weaviate-web/actions/workflows/action.yml/badge.svg)](https://github.com/toposoid/data-accessor-weaviate-web/actions/workflows/action.yml)|
| [data-accessor-redis-web](https://github.com/toposoid/data-accessor-redis-web)                                                         | This microservice is a CUID wrapper for [redis](https://github.com/redis/redis).                                                                                                                 |[![Test And Build](https://github.com/toposoid/data-accessor-redis-web/actions/workflows/action.yml/badge.svg)](https://github.com/toposoid/data-accessor-redis-web/actions/workflows/action.yml)|
| [data-accessor-mysql-web](https://github.com/toposoid/data-accessor-mysql-web)                                                         | This microservice is a CUID wrapper for [MySql](https://github.com/mysql/mysql-server).                                                                                                                 |[![Test And Build](https://github.com/toposoid/data-accessor-mysql-web/actions/workflows/action.yml/badge.svg)](https://github.com/toposoid/data-accessor-mysql-web/actions/workflows/action.yml)|
| [toposoid-contents-admin-web](https://github.com/toposoid/toposoid-contents-admin-web)                                                       |This microservice is responsible for managing content. Specifically, this includes image management. outputs the result in JSON.|[![Test And Build](https://github.com/toposoid/toposoid-contents-admin-web/actions/workflows/action.yml/badge.svg)](https://github.com/toposoid/toposoid-contents-admin-web/actions/workflows/action.yml)|
| [toposoid-common-image-recognition-web](https://github.com/toposoid/toposoid-common-image-recognition-web)        |This microservice is responsible for vectorizing data for image recognition. outputs the result in JSON.|[![Test And Build](https://github.com/toposoid/toposoid-common-image-recognition-web/actions/workflows/action.yml/badge.svg)](https://github.com/toposoid/toposoid-common-image-recognition-web/actions/workflows/action.yml)|
| [toposoid-feature-vectorizer](https://github.com/toposoid/toposoid-feature-vectorizer)                                                       | The main implementation of this module is text-to-vector representation conversion and search.                                                                                                            |[![Unit Test](https://github.com/toposoid/toposoid-feature-vectorizer/actions/workflows/action.yml/badge.svg)](https://github.com/toposoid/toposoid-feature-vectorizer/actions/workflows/action.yml)|
| [toposoid-deduction-common](https://github.com/toposoid/toposoid-deduction-common.git)                                                       | This is a common library used by toposoid developer in toposoid projects. In particular, this module is used by units that perform deductive reasoning in toposoid projects.                              |[![Unit Test Action](https://github.com/toposoid/toposoid-deduction-common/actions/workflows/action.yml/badge.svg)](https://github.com/toposoid/toposoid-deduction-common/actions/workflows/action.yml)|
| [toposoid-sentence-parser-japanese](https://github.com/toposoid/toposoid-sentence-parser-japanese.git)                                       | This component performs predicate argument structure analysis when a Japanese sentence is given as input. Then, it outputs the information necessary for converting to a knowledge graph.                 |[![Unit Test](https://github.com/toposoid/toposoid-sentence-parser-japanese/actions/workflows/action.yml/badge.svg)](https://github.com/toposoid/toposoid-sentence-parser-japanese/actions/workflows/action.yml)|
| [toposoid-knowledgebase-model](https://github.com/toposoid/toposoid-knowledgebase-model.git)                                                 | This library defines a basic model commonly used in toposoid projects.                                                                                                                                    |[![Header Check Action](https://github.com/toposoid/toposoid-knowledgebase-model/actions/workflows/action.yml/badge.svg)](https://github.com/toposoid/toposoid-knowledgebase-model/actions/workflows/action.yml)|
| [toposoid-deduction-protocol-model](https://github.com/toposoid/toposoid-deduction-protocol-model.git)                                       | This library defines a basic model commonly used in toposoid projects. Especially these are used in deductive logic.                                                                                      |[![Header Check Action](https://github.com/toposoid/toposoid-deduction-protocol-model/actions/workflows/action.yml/badge.svg)](https://github.com/toposoid/toposoid-deduction-protocol-model/actions/workflows/action.yml)|
| [toposoid-common](https://github.com/toposoid/toposoid-common.git)                                                                           | This is a common library used by toposoid developer in toposoid projects.                                                                                                                                 | [![Unit Test](https://github.com/toposoid/toposoid-common/actions/workflows/action.yml/badge.svg)](https://github.com/toposoid/toposoid-common/actions/workflows/action.yml)|
| [toposoid-test-utils](https://github.com/toposoid/toposoid-test-utils.git)                                                                           | This is a common library used by Linked Ideal LLC. in Scala projects. The main implementation of this project is Registering and deleting test data.                                                                                                                                 | [![Unit Test](https://github.com/toposoid/toposoid-test-utils/actions/workflows/action.yml/badge.svg)](https://github.com/toposoid/toposoid-test-utils/actions/workflows/action.yml)|
| [data-accessor-neo4j-web](https://github.com/toposoid/data-accessor-neo4j-web.git)                                               | This Microservice get information from Neo4J graph database. outputs the result in JSON.                                                                                                                  |[![Unit Test And Build Image Action](https://github.com/toposoid/data-accessor-neo4j-web/actions/workflows/action.yml/badge.svg)](https://github.com/toposoid/data-accessor-neo4j-web/actions/workflows/action.yml)|
| [scala-data-accessor-neo4j](https://github.com/toposoid/scala-data-accessor-neo4j.git)                                                       | The main implementation of this project is the neo4j driver Wrapper.                                                                                                                                      |[![Unit Test Action](https://github.com/toposoid/scala-data-accessor-neo4j/actions/workflows/action.yml/badge.svg)](https://github.com/toposoid/scala-data-accessor-neo4j/actions/workflows/action.yml)|
| [scala-common](https://github.com/toposoid/scala-common.git)                                                                                 | This is a common library used by Linked Ideal LLC. in Scala projects.                                                                                                                                     |[![Header Check Action](https://github.com/toposoid/scala-common/actions/workflows/action.yml/badge.svg)](https://github.com/toposoid/scala-common/actions/workflows/action.yml)|

## Requirements
* Docker version 24.0.x, or later
* docker-compose version 1.25.x

## Recommended environment For Standalone
* Required: at least 32GB of RAM
* Required: at least 100G of HDD(Total required Docker Image size)
* Please understand that since we are dealing with large models such as LLM, the Dockerfile size is large and the required machine SPEC is high.

## Setup For Standalone
```bssh
docker-compose up
```
* It takes more than 30 minutes to pull the Docker image for the first time.

## Usage
* Try accessing http://localhost:4444 in your browser.
* The UI has been confirmed to work only on Chrome browser.
### Knowledge data registration. You can register both text and images.
<img width="1760" alt="" src="https://github.com/toposoid/toposoid/assets/82787843/4e10ab60-08b2-422a-8dc6-15f17a1796b0">

### Knowledge data registration. You can also register via documents.
<img width="1760" alt="" src="https://github.com/user-attachments/assets/79454f3e-5fcf-4168-a604-d15b2e26737a" />

### Easy search. You can search both text and images.
<img width="1760" alt="" src="https://github.com/toposoid/toposoid/assets/82787843/c6e905ff-a295-4861-ad81-5c45dc51767d">


Try accessing http://localhost:7474 in your browser.
You will be able to see the data you registered from the API.
as follows
<img width="1604" alt="" src="https://github.com/toposoid/toposoid/assets/82787843/a4ccaafd-cda0-4060-9e1f-8ea9a0d04dbf">

### Deduction's Example
* During inference, it is possible to select units accordingly. Please set from the screen below.
<img width="1239" alt="" src="https://github.com/toposoid/toposoid/assets/82787843/2844fa7a-86c3-4cad-9f3c-6e6680590452">

### An example of a logic puzzle called a liar game

* Demo Web Application https://toposoid-service.com/

There are three people, A, B, and C, two honest people and the other one is a liar. And all three know who is honest and who is a liar. Here, an honest person is a person who always says the truth, and a liar is a person who always says the opposite of the truth. At this time, the following testimonies of A, B, and C were obtained.
* A's testimony: C is a liar.
* B's testimony: A is honest.
* C's testimony: B is a liar.
  Based on these testimonies, follow these steps to determine who is a liar.

This problem can be defined by one regulation and three hypothesis.
### regulation
* (A AND B AND NOT C) OR (A AND NOT B AND C) OR (NOT A AND B AND C)

|Step|Premise & Claim|LogicTree|
|-|-|-|
|1|![](https://user-images.githubusercontent.com/82787843/169679404-0785c371-68d6-4382-b5ab-36f6b7551dcc.png)|![](https://user-images.githubusercontent.com/82787843/169679431-df6cd49b-af7b-4295-87b8-a3d24ce766f1.png)|
|2|![](https://user-images.githubusercontent.com/82787843/169679492-ea6bcbd7-6199-4829-844c-7266f05ef85f.png)|![](https://user-images.githubusercontent.com/82787843/169679648-14d1084f-3b3e-4fbe-b6ad-388d4c7e9dcf.png)|
|3|![](https://user-images.githubusercontent.com/82787843/169679601-f248236d-60cc-4a72-b957-edbfd565de7f.png)|![](https://user-images.githubusercontent.com/82787843/169679665-17ec03f0-27b7-4c8c-9fda-470c323da235.png)|


### hypothesis
* A → NOT C
* B → A
* C → NOT B

|Step|Premise & Claim|LogicTree|
|-|-|-|
|4|![](https://user-images.githubusercontent.com/82787843/169679695-a110e6b4-b03f-448b-953d-26bf5c041c4b.png)|![](https://user-images.githubusercontent.com/82787843/169679711-4040e24a-7625-4c52-a60b-cd6d7a82c7bc.png)|
|5|![](https://user-images.githubusercontent.com/82787843/169679738-a766115b-e0aa-41b3-aecf-218713e690f1.png)|![](https://user-images.githubusercontent.com/82787843/169679740-00b26b8a-180b-4c9a-ada6-165c9f0e9478.png)|
|6|![](https://user-images.githubusercontent.com/82787843/169679754-eed0c88d-7452-4edb-9601-0d2c038d9d4a.png)|![](https://user-images.githubusercontent.com/82787843/169679755-4e0b213b-9892-42e8-960b-daafe1354752.png)|

### result
* Press the Analyze button to start logical inference.
<img width="1239" alt="" src="https://user-images.githubusercontent.com/82787843/169679810-3d821e14-ca85-4178-9926-da4b1cf84fb7.png">




## Note
* The memory allocated to Neo4J can be adjusted with NEO4J_dbms_memory_heap_max__size in docker-compose.yml.
* Services provided by Toposoid are accessible on port 4444
* Toposoid uses the [PDF Extract API](https://developer.adobe.com/document-services/docs/overview/pdf-extract-api/) provided by Adobe for document registration.The PDF Extract API can be used free of charge under the following conditions:https://developer.adobe.com/document-services/docs/overview/limits/#free-tier 
* In order to use The PDF Extract API, you need to create credentials. https://developer.adobe.com/document-services/apis/pdf-services/ After creating the credentials, please set the following environment variables in docker-compose.yml. TOPOSOID_PDF_SERVICES_CLIENT_ID TOPOSOID_PDF_SERVICES_CLIENT_SECRET 
* If you want to run in a remote environment or a virtual environment, change PRIVATE_IP_ADDRESS in docker-compose.yml according to your environment.


## License
This program is offered under a commercial and under the AGPL license.
For commercial licensing, contact us at https://toposoid.com/contact.  For AGPL licensing, see below.

AGPL licensing:
This program is free software: you can redistribute it and/or modify
it under the terms of the GNU Affero General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU Affero General Public License for more details.

You should have received a copy of the GNU Affero General Public License
along with this program.  If not, see <https://www.gnu.org/licenses/>.

## Author
* Makoto Kubodera([Linked Ideal LLC.](https://linked-ideal.com/))

Thank you!
