# WordPress Documentation Overview

This repository contains documentation for WordPress development and related topics written by developer AJC. This is not intended to be a comprehensive guide comparitive to official WP documentation, but personal notes and references from the developer's standpoint.

## Table of Contents

- [Main Resources](#main-resources)
- [Staging/Testing Setup](#stagingtesting-setup)

## Main Resources

**Official WordPress Documentation**

**Books**

## Staging/Testing Setup

Testing with WordPress involves some particular challenges. Setting up local testing environments from scratch with simple WP instances is a simple process, with tools like WAMP/MAMP, but this is not often representative of live instances.

Particulars in server configurations, plugins, themes, and other factors contribute to slight differences that can cause behavior in the testing instance that is not present in the live instance.

The following are some methods to set up staging/testing environments that can avoid this issue:

**Self-Hosting**

A good technique for setting up a testing environment is to configure a simple server on a local machine networked with the main development machine. This allows full control over the server environment configuration. Any extra PC can be used for this purpose, but often a device like a Raspberry Pi can be used for this purpose.

An alternative approach to this is to use virtual machines.

The main downside to this approach is that it requires a separate machine to be running at all times during development. Maintaining up-time and ensuring that the server is accessible to any other developers not connected to the LAN are specific challenges.

**Third-Party Hosting via Secondary Mirror Instances**

Creating a second instance of the live server on a separate host is another approach. This can be done with a subdomain or a separate domain. This approach is more costly than self-hosting, but it can be more reliable and accessible.

One of the key challenges is insuring that the secondary instance mirrors the same server configuration as the live instance. This can be done with tools like WP Migrate DB Pro, but it is not always perfect.

The main advantage of this approach is that it is more accessible to other developers and clients, and it can be more reliable than self-hosting.