---
title: plugin stop
categories: |
  core
version: 0.92.0
core: |
  Stop an installed plugin if it was running.
usage: |
  Stop an installed plugin if it was running.
feature: default
---
<!-- This file is automatically generated. Please edit the command in https://github.com/nushell/nushell instead. -->

# `plugin stop` for [core](/commands/categories/core.md)

<div class='command-title'>Stop an installed plugin if it was running.</div>

## Signature

```> plugin stop {flags} (name)```

## Parameters

 -  `name`: The name of the plugin to stop.


## Input/output types:

| input   | output  |
| ------- | ------- |
| nothing | nothing |

## Examples

Stop the plugin named `inc`.
```nu
> plugin stop inc

```

Stop all plugins.
```nu
> plugin list | each { |p| plugin stop $p.name }

```