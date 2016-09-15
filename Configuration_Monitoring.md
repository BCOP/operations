# Configuration Monitoring

## Overview

Configuration monitoring systems perform a seemingly trivial task. After being configured with one or more targets, typically a physical or virtual network element, such systems regularly download the current configuration of the target, compare it to the previously stored configuration, and archive any changes. Optionally, an operator is notified of any changes that occured by e-mail or via  another channel.

The presence of a configuration monitoring system in a modern, fully-automated, lifecycle managed AS may appear counter-intuitive. In an AS that employs change management, utilizes generated configuration from standard templates and enriches these templates with provisioning data from OSS and BSS systems, any configuration end-product can be simply re-generated and monitoring or archiving specific device configuration might appear pointless.

Few ASes, however, operate completely within such perfectly controlled conditions, and even under such conditions, configuration monitoring may offer some benefits.

For ASes employing artisan configuration (operator written, often on the device itself), the advantages of configuration archiving are numerous:

* Provides a backup of network elements configuration for disaster recovery
* Creates a central archive of configuration files for further processing
* Allows teams to track changes as they are applied by individual team members

Even in partially or fully automated ASes, however, configuration monitoring systems may still offer a number of benefits:

* Assists in identifying operator tampering and archives temporary hacks
* Assists in identifying mismatches between desired generated configuration and applied effective configuration
* Can optionally collect and archive certain forms of telemetry from network elements, such as debugging information, which may be inaccessible via other channels (such as regular execution of undocumented debugging information generating commands)

## Recommendations

* [Oxidized](https://github.com/ytti/oxidized) - A modern configuration monitoring system offering easy integration capabilities, a web interface, and broad support for a large array of network elements. Self-hosted.
* [RANCID](http://www.shrubbery.net/rancid/) - An old favorite with an extensive library of supported network elements. Self-hosted.

## Do and Don't

### Do:
* Archive your ASes configuration, as well as configuration of end-user CPEs. Consider offering configuration monitoring as a service in a service provider environment.

* Archive full and usable configuration including passwords if you operate configuration monitoring in a secure environment and backed by secure storage - while removing passwords and other sensitive information from archived configuration may appeal appealing at first, it considerably complicates the process of utilizing the archive as a backup of last resort.

### Don't:
* Don't provide the configuration monitoring system an unrestricted administrative account on network elements. Instead, create a dedicated read-only account that allows configuration harvesting but prohibits changes. The same account can be reused for additional information gathering interfaces such as a looking glass or CLI route server access.
