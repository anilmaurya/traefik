# Zipkin

To enable the Zipkin:

```toml tab="File (TOML)"
[tracing]
  [tracing.zipkin]
```

```yaml tab="File (YAML)"
tracing:
  zipkin: {}
```

```bash tab="CLI"
--tracing.zipkin=true
```

#### `httpEndpoint`

_Required, Default="http://localhost:9411/api/v1/spans"_

Zipkin HTTP endpoint used to send data.

```toml tab="File (TOML)"
[tracing]
  [tracing.zipkin]
    httpEndpoint = "http://localhost:9411/api/v1/spans"
```

```yaml tab="File (YAML)"
tracing:
  zipkin:
    httpEndpoint: http://localhost:9411/api/v1/spans
```

```bash tab="CLI"
--tracing.zipkin.httpEndpoint="http://localhost:9411/api/v1/spans"
```

#### `debug`

_Optional, Default=false_

Enable Zipkin debug.

```toml tab="File (TOML)"
[tracing]
  [tracing.zipkin]
    debug = true
```

```yaml tab="File (YAML)"
tracing:
  zipkin:
    debug: true
```

```bash tab="CLI"
--tracing.zipkin.debug=true
```

#### `sameSpan`

_Optional, Default=false_

Use Zipkin SameSpan RPC style traces.

```toml tab="File (TOML)"
[tracing]
  [tracing.zipkin]
    sameSpan = true
```

```yaml tab="File (YAML)"
tracing:
  zipkin:
    sameSpan: true
```

```bash tab="CLI"
--tracing.zipkin.sameSpan=true
```

#### `id128Bit`

_Optional, Default=true_

Use Zipkin 128 bit root span IDs.

```toml tab="File (TOML)"
[tracing]
  [tracing.zipkin]
    id128Bit = false
```

```yaml tab="File (YAML)"
tracing:
  zipkin:
    id128Bit: false
```

```bash tab="CLI"
--tracing.zipkin.id128Bit=false
```

#### `sampleRate`

_Required, Default=1.0_

The rate between 0.0 and 1.0 of requests to trace.

```toml tab="File (TOML)"
[tracing]
  [tracing.zipkin]
    sampleRate = 0.2
```

```yaml tab="File (YAML)"
tracing:
  zipkin:
    sampleRate: 0.2
```

```bash tab="CLI"
--tracing.zipkin.sampleRate="0.2"
```