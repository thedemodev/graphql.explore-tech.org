---
path: '/materials/light-graphql-4j'
type: 'GitHub'
img: './screenshot.png'
material:
  title: 'light-graphql-4j'
  url: 'https://github.com/networknt/light-graphql-4j'
  github_url: 'https://github.com/networknt/light-graphql-4j'
  subscribers_count: '10'
  stargazers_count: '13'
  tags: ['graphql','graphql-security','graphql-validator','java','relay','relayjs','security']
  subtitle: 'GraphQL implementation based on light-4j'
  clone_url: 'https://github.com/networknt/light-graphql-4j.git'
  ssh_url: 'git@github.com:networknt/light-graphql-4j.git'
  pushed_at: '2019-01-14T21:20:33Z'
  updated_at: '2019-01-13T17:40:21Z'
  author:
    name: 'networknt'
    avatar: 'https://avatars2.githubusercontent.com/u/8740739?v=4'
    github_url: 'https://github.com/networknt'
  latestRelease:
    tag_name: '1.5.28'
    name: '1.5.28'
    url: 'https://github.com/networknt/light-graphql-4j/releases/tag/1.5.28'
    created_at: '2019-01-13T17:40:17Z'
---
GraphQL framework based on light-4j

[Developer Chat](https://gitter.im/networknt/light-graphql-4j) |
[Documentation](https://doc.networknt.com/style/light-graphql-4j/) |
[Contribution Guide](CONTRIBUTING.md) |

[![Build Status](https://travis-ci.org/networknt/light-graphql-4j.svg?branch=master)](https://travis-ci.org/networknt/light-graphql-4j)

## Components

### graphql-common
This module controls the configuration for GraphQL service and share some static variables
with other modules to make the dependencies much simpler. 

### graphql-router
This module provides RouteHandler and SchemaProvider interfaces and implement both GET and
POST handlers for GraphQL. 

## Middleware Handlers:

### graphql-security
This is the handler that should be put before graphql-validator. There is no need to
do any validation if JWT token does not exist in the request header.

### graphql-validator
Basic request validation for the graphql path and methods. It is the first line of
validation right after graphql-security and it doesn't have any knowledge about the
graphql query parameter and body.

## Tutorial

### [Hello World](https://doc.networknt.com/tutorial/graphql/helloworld/)

This is a very simple Hello World query to show you how to get GraphQL up and running with
light-codegen without using GraphQL IDL.

### [Star Wars](https://doc.networknt.com/tutorial/graphql/starwars/)

This is a similar example as Hello World with IDL to trigger the generation. It is utilize the
star wars GraphQL IDL downloaded from the Internet.
 
### [Mutation](https://doc.networknt.com/tutorial/graphql/mutation/)

This example shows you how to create a full blown GraphQL service with both query and mutation.

### [Mutation IDL](https://doc.networknt.com/tutorial/graphql/mutation-idl/)

This is the same example like the mutation but is generated from a schema. 

### [Relay Todo](https://doc.networknt.com/tutorial/graphql/relay-todo/)

This is to show you how to build a GraphQL service that is working with Relayjs. 

