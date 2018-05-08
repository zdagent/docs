<!--
title: 22 - About audit reports
featured: true
-->

# About audit reports

Audit reports contain information about security vulnerabilities in your project's dependencies to help you fix the vulnerability or troubleshoot further.

The fields in an audit report are:

* [Severity](#severity)
* [Description](#description)
* [Package](#package)
* [Patched in](#patched-in)
* [Dependency of](#dependency-of)
* [Path](#path)
* [More info](#more-info)

```
┌───────────────┬──────────────────────────────────────────────────────────────┐
│ high          │ Denial of Service                                            │
├───────────────┼──────────────────────────────────────────────────────────────┤
│ Package       │ foo                                                          │
├───────────────┼──────────────────────────────────────────────────────────────┤
│ Patched in    │ No patch available                                           │
├───────────────┼──────────────────────────────────────────────────────────────┤
│ Dependency of │ @npm/spife                                                   │
├───────────────┼──────────────────────────────────────────────────────────────┤
│ Path          │ @npm/spife > numbat-process > numbat-emitter > foo           │
├───────────────┼──────────────────────────────────────────────────────────────┤
│ More info     │ https://nodesecurity.io/advisories/550                       │
└───────────────┴──────────────────────────────────────────────────────────────┘
```

## Severity

The severity of the vulnerability, determined by the impact and exploitability of the vulnerability in its most common use case.

| Severity |  Recommended action |
|----------|---------------------|
| Critical | Address immediately |
| High | Address as quickly as possible |
| Moderate | Address as time allows |
| Low | Address at your discretion |

## Description

The description of the vulnerability. For example, "Denial of service".

## Package

The name of the package that contains the vulnerability.

## Patched in

The semantic version range that describes which versions contain a fix for the vulnerability.

## Dependency of

The module that the package with the vulnerability depends on.

## Path

The path to the code that contains the vulnerability.

## More info

A link to the security report.
