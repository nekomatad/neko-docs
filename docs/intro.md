---
sidebar_position: 1
---

# Intro
Nekomata is free application daemonizer, deployer and manager, which was developed with permutability in mind. It is created to replace tools such as pm2 or supervisord and provide extensibility by supporting user plugins and having ability to replace even core features with extensions and plugins.
# Structure
Each part of the functionality is implemented by a specific plugin, which most often has two parts - "standard" and "implementation". Also, there are modules and extensions. A structure description is essentially a specification that developers adhere to when designing extensions to fit into the plugin ecosystem. We recommend reading the [Developing plugins](category/developing-plugins) section even if you don’t plan to develop plugins, as it can greatly simplify understanding of the plugin installation process and how the configuration works
# Installation
Since nekomata does not have a core, an installer is needed that will drop the entry point and immediately install the basic plugins that are necessary to interact with the application. We provide a minimal official pack of plugins, as well as a selection of additional ones that may be useful for quick installation on a client or server.
Some plugins (for example, those that act as plugin managers or loaders) are forced to have some rules for other plugins installed on the system. Accordingly, this documentation describes working with nekomata installations that are based on the official pack. There may be other implementations for the internal core functions or alternative core packs. In this case, you will have to refer to the documentation provided by their developer.