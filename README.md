# iDAI.world core

iDAI.world core is the basic datamodel used to aggregate information on the
data in the several heterogenous applications of the iDAI.world.

## Repository structure

The main ontology can be found in the root folder and can be edited using Protégé.

This repository also contains *examples* for the application of this ontology
as JSON files.

The folder *contexts* contains JSON-LD context definitions that can be used
to generate linked data in different flavours.

## Basic principles

### Simplicity

The base class **Entity** contains most of the available attributes to describe
all kinds of resources in a compatible way. All other attributes from source
systems that can not be mapped to one of these basic attributes should be 
aggregated in the **description** field.

### Relations

All entities should be described in terms of the basic relations that answer
the questions *what*, *where* and *when*. These concepts are represented by
the respective classes **Subject**, **Place** and **Period**.

### Datasets

The class **Dataset** can be used to create identifiable collections of digital
resources. These may for example serve as entry points for project sites and can
also be nested hierarchically to implement a catalog structure.

Datasets can also be used provide metadata about collections of data that have not
been mapped on an item-level.

### Distinction between entities and the digital documents they are described in

Along the lines of the principles for [Cool URIs](https://www.w3.org/TR/cooluris/)
the iDAI.world core Ontology distinguishes between physical and immaterial entities
and the electronic resources that contain metadata and data about these.
