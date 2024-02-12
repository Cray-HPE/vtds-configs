# Configuration Overlays for vTDS Systems

## Configuration Sources

Each layer of a vTDS system comes with a base configuration that
contains all of the default values that can be used to construct the
vTDS at that layer. The full vTDS system configuration is completed by
overlaying YAML configuration overlay files from various configuration
sources onto the base configuration of each layer.

The four layers that make up a vTDS system are:

* Application
* Cluster
* Platform
* Provider

At each of these four layers, there are layer implementations that are
specific to the technology being used at that layer. For example,
there might be a GCP provider layer and an OpenStack provider
layer. Each layer also needs a configuration overlay to configure the
layer for the intended purpose of the vTDS system to be constructed.

The configuration filles found in this repository provide
configuration sources for vTDS systems that are applicable to HPE use
cases. The layer configurations are kept in sub-directories of the
'layers' dirtectory here, one sub-directory for each of the four kinds
of layer listed above.

## Sample Core Configurations

In addition to layer configurations, there are 'Core Configurations'
which drive both the selection of layers for a given vTDS and the
selection of configuration sources. The 'core-configs' sub-directory
here provides a set of sample core configurations that a user might
use or modify to set up a new vTDS system.
