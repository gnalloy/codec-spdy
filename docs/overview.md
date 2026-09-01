# Overview

[简体中文](overview.zh-CN.md) | [Docs Index](README.md)

## Purpose

SPDY frame codec support for legacy protocol interop in Gnalloy pipelines.

This module sits above transports and below application handlers. It translates bytes or Gnalloy messages into protocol objects, and translates outbound protocol objects back to bytes. It does not open sockets or own EventLoops.

## Repository Identity

- Module path: `gnalloy.org/codec-spdy`
- GitHub repository: `github.com/gnalloy/codec-spdy`
- Default branch: `dev`
- License: Apache-2.0

## Package Map
- `gnalloy.org/codec-spdy` (`spdy`)

## Direct Gnalloy Dependencies
- `gnalloy.org/gnalloy`

## Direct Dependents in the Current Module Plan
- No repository in the current module plan depends on this module directly.

## Architecture Position

Gnalloy keeps the core small and dependency-light. This repository is a replaceable module around one responsibility, connected through explicit Go packages instead of runtime discovery.

## Compatibility

The public import path is `gnalloy.org/codec-spdy`. Until the first stable tag is published, use `@dev` or an explicit pseudo-version selected by your dependency policy.
