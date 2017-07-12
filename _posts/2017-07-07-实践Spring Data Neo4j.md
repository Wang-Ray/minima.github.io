---
layout: post
title: "实践Spring Data Neo4j"
date: 2017-07-07 09:00:00 +0800
categories: database nosql neo4j
tags: database nosql neo4j spring-data-neo4j
---

Spring Data Neo4j注解

| 注解                   | 描述                                       |
| -------------------- | ---------------------------------------- |
| @NodeEntity          | Node，默认Label为类名                          |
| @RelattionShipEntity | RelationShip，默认type为类名，一般而言，带属性的relationShip（rich relationShip）才有必要建立RelationShipEntity |
| @StartNode           |                                          |
| @EndNode             |                                          |
| @Fetch               |                                          |
| @GraphId             | neo4j ID                                 |
| @GraphProperties     |                                          |
| @GraphTraversal      |                                          |
| @Indexed             | 声明某个属性应该被索引（schema indexing）             |
| @Labels              | Label                                    |
| @Query               |                                          |
| @QueryResult         |                                          |
| @RelatedTo           | Set/List/Collection/Iterable (read-only)/<NodeEntity>，用于basic relationShip，默认type为域名，此时可以不需要使用@RelateTo |
| @RelatedToVia        | Set/List/Collection/Iterable (read-only)/<RelattionShipEntity>，用于rich relationShip，默认type从RelattionShipEntity推断 |
| @RelationShipType    | ReletionShipType                         |
| @ResultColumn        |                                          |