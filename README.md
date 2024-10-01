# README

## Overview

This project focuses on constructing and manipulating **functional images** using **Haskell**. It demonstrates functional programming principles such as **lazy evaluation**, **higher-order functions**, and explores the distinction between **shallow embedding** and **deep embedding**. The project is divided into multiple stages, each advancing the concepts of regions, transformations, and optimizations in functional image processing.

## Stages

### Shallow Embedding
- **Region Representation**: Regions are defined using **characteristic functions**. These functions determine whether a point belongs to a specific region, such as a circle or rectangle.
- **Transformation Representation**: This stage introduces basic transformations (e.g., translations and scaling) that can be applied to regions.
- **Operations**: Operations like union, intersection, and complement of regions are implemented using **list comprehensions**.
- **Lazy Evaluation**: Ensures that computations are deferred until absolutely necessary, allowing for efficient processing of large or infinite regions.
  
### Deep Embedding
- **Abstract Syntax Tree (AST)**: Transition to **deep embedding**, where regions and transformations are represented as an **AST**. This allows for flexible interpretations and optimizations.
- **Smart Constructors**: These constructors simplify the manipulation of ASTs by providing easier ways to compose and combine transformations.
- **Optimization**: Introduces optimization strategies, such as combining consecutive transformations (e.g., merging two translations into one).

### Optimization and Folding
- **Folding Over AST**: In this stage, the project focuses on using **folding** techniques over the AST to simplify complex operations on regions and transformations.
- **Optimizing Transformations**: Optimizations include merging redundant transformations and applying transformations to simplify regions' representation.