# API Reference

[简体中文](api.zh-CN.md) | [Docs Index](README.md)

This inventory is generated from `go doc -short` for the packages in this repository. It is a quick public-surface map; source files and tests remain the authority for exact semantics.

## Packages

### `gnalloy.org/codec-spdy`

Package name: `spdy`

```text
const Version3 uint16 = 3 ...
const FlagFIN byte = 0x01 ...
var ErrInvalidFrame = errors.New("spdy: invalid frame") ...
type DataFrame struct{ ... }
type Decoder struct{ ... }
    func NewDecoder(version uint16, maxFrameLength int) (*Decoder, error)
type Encoder struct{ ... }
    func NewEncoder(version uint16) *Encoder
type FrameType uint16
    const FrameTypeData FrameType = 0 ...
type GoAwayFrame struct{ ... }
type HeadersFrame struct{ ... }
type PingFrame struct{ ... }
type RSTStreamFrame struct{ ... }
type Setting struct{ ... }
type SettingsFrame struct{ ... }
type SynReplyFrame struct{ ... }
type SynStreamFrame struct{ ... }
type UnknownFrame struct{ ... }
type WindowUpdateFrame struct{ ... }
```
