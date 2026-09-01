# API 参考

[English](api.md) | [文档索引](README.zh-CN.md)

本清单由本仓库 package 的 `go doc -short` 生成，用于快速查看公共面。精确语义以源码和测试为准。

## 包

### `gnalloy.org/codec-spdy`

包名：`spdy`

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
