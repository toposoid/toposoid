# Toposoid Community Edition
Toposoid is a knowledge base construction platform.
Toposoid has the following features.
* You can build a knowledge base just by entering sentences (currently only Japanese is supported).
* If you enter the text as it is, you can search the knowledge base and obtain inference results.
* This inferring program is designed so that developers can freely extend and replace it in their favorite programming language.

In this repository, it is published as Toposoid Community Edition. For more information -> https://toposoid.com/

## Outline Drawing
<img width="1760" alt="2021-10-04 21 20 01" src="https://user-images.githubusercontent.com/82787843/135850589-0df6b747-df02-435d-9992-ee1831fec916.png">

## Knowledge Base Image
<img width="1747" alt="2021-10-05 12 24 49" src="https://user-images.githubusercontent.com/82787843/135955167-4cbed1eb-a423-4201-82b7-743d37664184.png">

## Toposoid project dependencies
<img width="1768" alt="2021-10-04 21 22 14" src="https://user-images.githubusercontent.com/82787843/135850618-15658ad2-66ef-4e26-bb9d-f4c3d32a3920.png">

| ProjectName | Function | Status |
| - | - | - |
| toposoid | Root project for all Toposoid projects |
| [toposoid-component-dispatcher-web](https://github.com/toposoid/toposoid-component-dispatcher-web.git) | This microservice integrates two major microservices. One is a microservice that analyzes the predicate argument structure of sentences, and the other is a microservice that makes logical inferences. | [![Unit Test And Build Image Action](https://github.com/toposoid/toposoid-component-dispatcher-web/actions/workflows/action.yml/badge.svg?branch=main)](https://github.com/toposoid/toposoid-component-dispatcher-web/actions/workflows/action.yml) |
| [toposoid-knowledge-register-web](https://github.com/toposoid/toposoid-knowledge-register-web.git) |This Microservice registers the results of predicate argument structure analysis of Japanese natural sentences in a graph database.  | [![Unit Test And Build Image Action](https://github.com/toposoid/toposoid-knowledge-register-web/actions/workflows/action.yml/badge.svg?branch=main)](https://github.com/toposoid/toposoid-knowledge-register-web/actions/workflows/action.yml) |
| [toposoid-sentence-parser-japanese-web](https://github.com/toposoid/toposoid-sentence-parser-japanese-web.git) | This Microservice analyzes the predicate argument structure of Japanese sentences and outputs the result in JSON.  |[![Test And Build](https://github.com/toposoid/toposoid-sentence-parser-japanese-web/actions/workflows/action.yml/badge.svg)](https://github.com/toposoid/toposoid-sentence-parser-japanese-web/actions/workflows/action.yml)|  
| [toposoid-common-nlp-japanese-web](https://github.com/toposoid/toposoid-common-nlp-japanese-web.git) |This Microservice provides an NLP function that handles Japanese and outputs the result in JSON.|[![Test And Build](https://github.com/toposoid/toposoid-common-nlp-japanese-web/actions/workflows/action.yml/badge.svg)](https://github.com/toposoid/toposoid-common-nlp-japanese-web/actions/workflows/action.yml)|
| [toposoid-sentence-parser-english-web](https://github.com/toposoid/toposoid-sentence-parser-english-web.git)|This Microservice analyzes dependency's structure of English sentences and outputs the result in JSON.|[![Test And Build](https://github.com/toposoid/toposoid-sentence-parser-english-web/actions/workflows/action.yml/badge.svg)](https://github.com/toposoid/toposoid-sentence-parser-english-web/actions/workflows/action.yml)|
| [toposoid-common-nlp-english-web](https://github.com/toposoid/toposoid-common-nlp-english-web.git)|This Microservice provides an NLP function that handles English and outputs the result in JSON.|[![Test And Build](https://github.com/toposoid/toposoid-common-nlp-english-web/actions/workflows/action.yml/badge.svg)](https://github.com/toposoid/toposoid-common-nlp-english-web/actions/workflows/action.yml)|
| [toposoid-deduction-admin-web](https://github.com/toposoid/toposoid-deduction-admin-web.git) | This microservice provides the ability to manage multiple deductive inference logic to register, update microservices.  |[![Unit Test And Build Image Action](https://github.com/toposoid/toposoid-deduction-admin-web/actions/workflows/action.yml/badge.svg?branch=main)](https://github.com/toposoid/toposoid-deduction-admin-web/actions/workflows/action.yml)|  
| [toposoid-deduction-unit-exact-match-web](https://github.com/toposoid/toposoid-deduction-unit-exact-match-web.git) | This microservice provides the ability to determine if the text you enter matches the knowledge graph exactly. 　|[![Unit Test And Build Image Action](https://github.com/toposoid/toposoid-deduction-unit-exact-match-web/actions/workflows/action.yml/badge.svg?branch=main)](https://github.com/toposoid/toposoid-deduction-unit-exact-match-web/actions/workflows/action.yml)| 
| [toposoid-deduction-unit-synonym-match-web](https://github.com/toposoid/toposoid-deduction-unit-synonym-match-web.git　) | This microservice provides the ability to determine if the text you enter matches, provided that the knowledge graph and synonyms are equated. |[![Unit Test And Build Image Action](https://github.com/toposoid/toposoid-deduction-unit-synonym-match-web/actions/workflows/action.yml/badge.svg?branch=main)](https://github.com/toposoid/toposoid-deduction-unit-synonym-match-web/actions/workflows/action.yml)|
| [toposoid-deduction-common](https://github.com/toposoid/toposoid-deduction-common.git) | This is a common library used by toposoid developer in toposoid projects. In particular, this module is used by units that perform deductive reasoning in toposoid projects.  |[![Unit Test Action](https://github.com/toposoid/toposoid-deduction-common/actions/workflows/action.yml/badge.svg?branch=main)](https://github.com/toposoid/toposoid-deduction-common/actions/workflows/action.yml)|
| [toposoid-sentence-parser-japanese](https://github.com/toposoid/toposoid-sentence-parser-japanese.git) | This component performs predicate argument structure analysis when a Japanese sentence is given as input. Then, it outputs the information necessary for converting to a knowledge graph.  |[![Unit Test](https://github.com/toposoid/toposoid-sentence-parser-japanese/actions/workflows/action.yml/badge.svg)](https://github.com/toposoid/toposoid-sentence-parser-japanese/actions/workflows/action.yml)|
| [toposoid-knowledgebase-model](https://github.com/toposoid/toposoid-knowledgebase-model.git) | This library defines a basic model commonly used in toposoid projects.  |[![Header Check Action](https://github.com/toposoid/toposoid-knowledgebase-model/actions/workflows/action.yml/badge.svg?branch=main)](https://github.com/toposoid/toposoid-knowledgebase-model/actions/workflows/action.yml)|
| [toposoid-deduction-protocol-model](https://github.com/toposoid/toposoid-deduction-protocol-model.git) | This library defines a basic model commonly used in toposoid projects. Especially these are used in deductive logic.  |[![Header Check Action](https://github.com/toposoid/toposoid-deduction-protocol-model/actions/workflows/action.yml/badge.svg?branch=main)](https://github.com/toposoid/toposoid-deduction-protocol-model/actions/workflows/action.yml)|
| [toposoid-common](https://github.com/toposoid/toposoid-common.git) | This is a common library used by toposoid developer in toposoid projects.  | [![Unit Test](https://github.com/toposoid/toposoid-common/actions/workflows/action.yml/badge.svg)](https://github.com/toposoid/toposoid-common/actions/workflows/action.yml)|
| [scala-data-accessor-neo4j-web](https://github.com/toposoid/scala-data-accessor-neo4j-web.git) | This Microservice get information from Neo4J graph database. outputs the result in JSON.  |[![Unit Test And Build Image Action](https://github.com/toposoid/scala-data-accessor-neo4j-web/actions/workflows/action.yml/badge.svg?branch=main)](https://github.com/toposoid/scala-data-accessor-neo4j-web/actions/workflows/action.yml)|
| [scala-data-accessor-neo4j](https://github.com/toposoid/scala-data-accessor-neo4j.git)| The main implementation of this project is the neo4j driver Wrapper. |[![Unit Test Action](https://github.com/toposoid/scala-data-accessor-neo4j/actions/workflows/action.yml/badge.svg?branch=main)](https://github.com/toposoid/scala-data-accessor-neo4j/actions/workflows/action.yml)|
| [scala-common](https://github.com/toposoid/scala-common.git) | This is a common library used by Linked Ideal LLC. in Scala projects.  |[![Header Check Action](https://github.com/toposoid/scala-common/actions/workflows/action.yml/badge.svg)](https://github.com/toposoid/scala-common/actions/workflows/action.yml)|


## Requirements
* Docker version 20.10.x, or later
* docker-compose version 1.22.x

## Recommended environment
* Required: at least 8GB of RAM (The maximum heap memory size of the JVM is set to 6G (Application: 4G, Neo4J: 2G))
* Required: 65G or higher of HDD

## Setup
```bssh
docker-compose up -d
```
It takes more than 20 minutes to pull the Docker image for the first time.
## Usage
```bash
# Regist knowledge
# Japanese
curl -X POST -H "Content-Type: application/json" -d '{"knowledgeList":[{"sentence":"案ずるより産むが易し。", "lang": "ja_JP", "extentInfoJson":"{}"}]}' http://localhost:9002/regist
# English
curl -X POST -H "Content-Type: application/json" -d '{"knowledgeList":[{"sentence":"Our life is our art.", "lang": "en_US", "extentInfoJson":"{}"}]}' http://localhost:9002/regist
```
Try accessing http://localhost:7474 in your browser.
You will be able to see the data you registered from the API.
as follows
<img width="1755" alt="スクリーンショット 2022-01-08 19 31 10" src="https://user-images.githubusercontent.com/82787843/148640948-005c12d4-17dd-49dc-95fb-b3e4b6d8b0d6.png">

```bash
# Deduction
# Japanese
curl -X POST -H "Content-Type: application/json" -d '{"premise":[],"claim":[{"sentence":"案ずるより産むが易し。", "lang": "ja_JP", "extentInfoJson":"{}"}]}' http://localhost:9004/analyze
# English
curl -X POST -H "Content-Type: application/json" -d '{"premise":[],"claim":[{"sentence":"Our life is our art.", "lang": "en_US", "extentInfoJson":"{}"}]}' http://localhost:9004/analyze
```
<img width="1179" alt="2021-10-05 12 12 08" src="https://user-images.githubusercontent.com/82787843/135954527-25c16a6b-b50a-4783-a5c0-1b8b4062d453.png">

## Note
* If you want to run in a remote environment or a virtual environment, change PRIVATE_IP_ADDRESS in docker-compose.yml according to your environment.
* The memory allocated to Neo4J can be adjusted with NEO4J_dbms_memory_heap_max__size in docker-compose.yml.


## License
Toposoid Community Edition is an open source product licensed under Apache-2.0 License.
But, the license of Neo4J used by Toposoid Community Edition as a graph database is GPLv3. Please be careful.
If you use Neo4j Enterprise Edition, this limitation is removed. Currently,
we are working on making the licensed Topsoid Enterprise Edition including the above available soon.

## Author
* Makoto Kubodera([Linked Ideal LLC.](https://linked-ideal.com/))

Thank you!
