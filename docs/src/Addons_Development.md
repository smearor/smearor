# Addon Development

Goal is to make as much as possible low code.

## Functionality

* Provide assets (Images, CSS, JavaScript, Fonts)
* Provide widgets
* Provide data models
    * Components
    * Entity Types
    * Relation Types
* Provide data sources
    * HTTP
    * MQTT
    * GraphQL
* Provide data sinks
    * HTTP
    * MQTT
    * GraphQL
* Provide control flow logic
    * Flow Types
    * Flow Instances

## Architecture 

### Data Flow (Output)

1. Data Source -> Entity -> GraphQL -> Widget Content
2. Data Source -> Entity -> Flow -> Entity -> GraphQL -> Widget Content

### Data Flow (Input)

1. Widget Action -> GraphQL -> Entity
2. Widget Action -> GraphQL -> Entity -> Flow
3. Widget Action -> GraphQL -> Entity -> Data Sink
4. Widget Action -> GraphQL -> Entity -> Flow -> Entity -> Data Sink

### Data Flow (InOut)

1. Widget Action -> GraphQL -> Entity -> Flow -> Entity -> GraphQL -> Widget Content
2. Widget Action -> GraphQL -> Entity -> Flow -> Data Sink -> Data Source -> Entity -> GraphQL -> Widget Content
