![iCargo-API logo](images/iCargo-API-64.png) iCargo-API (version 1.0)
==========

The iCargo API is an [entity-centric](docs/entity.md) HTTP REST interface for the exchange of information with and within the [iCargo ecosystem]() to be used by iCargo [Access Points](). These Access Points require a [ontology]() as configuration because the iCargo API is based on [semantics](https://en.wikipedia.org/wiki/Semantics).  

## Context
The [iCargo ecosystem]() is a federation of distributed and independent systems, designed to support Transport Logistics with the exchange of information between organisations across the Supply Chain. [Access Points]() are software services which support the iCargo API and provide a single entry point for an organisation to the iCargo ecosystem. One of the characteristics of this ecosystem is controlled and secure exchange of information without the need for a centralised controlling system or organisation.

The iCargo REST API can be implemented as symmetrical software modules called inbound and outbound [connectors](docs/connectors.md) at the beginning or at the end of a pipeline of software services. The concepts of inbound and outbound connectors are required to distinguish a [synchronous](docs/connectors.md#synchrone-vs-asynchrone) response from an [asynchronous](docs/connectors.md#synchrone-vs-asynchrone) response.

[![Pipeline of software services](images/pipeline.png)](docs/connectors.md)

This API specification and the iCargo ecosystem are developed by the [iCargo project](http://i-cargo.eu/).

## Content
This specification describes the following topics:
*  [Capabilities](#capabilities), an overview of the functionality;
*  [Information model](#model), required for addressing (REST) resources and describes how the resources and their status shall be modelled in a knowledge base; 
*  [Generic specification](#generic), applicable for all API calls such as mandatory HTTP-header attributes and the path structure of the URL;
*  [Access restrictions](#access), authorisation requirements related to the different types and roles identified for an actor;
*  [Function specific specification](#specific), a detailed description for each HTTP call of the path to a resource, how to use the header attributes and the expected result.

## <a name="capabilities"></a>Capabilities
The Entity-centric Services interface [IES] supports the following [entity-centric](docs/entity.md) specific capabilities of an Access Point:
*  To create and register an entity;
*  To search for an entity and discover which Access Points can provide information; 
*  To provide information about a concept or entity;
*  To perform an entity related action such as publish/subscribe;
*  To change or update the attributes an entity including relations to other entities;
*  To delete an entity.

Additionally, the following capabilities are supported as well:
*  To support invitations for cooperation;
*  To provide information about the Access Point itself;
*  To route information to other software services as part of a workflow;
* To support life cycle management of concepts and entities and their states.

Section E4 will elaborate how each capability is supported per API call.

## <a name="model"></a>Information model

## <a name="generic"></a> Generic specification

### Path

### Header

### Body
The body of all iCargo compliant requests and responses is a uniform JSON data structure using UTF-8 character encoding. This enables a uniform way for creating request and processing responses and results in less code and bugs.
For an in depth description of the [iCargo body data structure](docs/body.md) click [here](docs/body.md).

## <a name="access"></a>Access restrictions

## <a name="specific"></a>Functional specific request

## Contributions
[![iCargo logo](images/iCargoLogo-320.png)](http://i-cargo.eu/).


