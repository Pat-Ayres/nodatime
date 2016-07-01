The [`Instant`](../api/NodaTime.Instant.yml) type supports the following patterns:

Standard Patterns
-----------------

The following standard pattern is supported:

- `g`: General format pattern.  
  The ISO-8601 representation of this instant in UTC, using the
  pattern "uuuu-MM-ddTHH:mm:ss'Z'" and always using the invariant culture,
  with the default "start of time" and "end of time" labels.
  This is the default format pattern.

Custom Patterns
---------------

[`Instant`](../api/NodaTime.Instant.yml) supports all the [`LocalDateTime` custom patterns](localdatetime-patterns.md).
The pattern allows the culture to be specified, but *always* uses the ISO-8601 calendar, and *always* uses the UTC
time zone. The "template value" is always the unix epoch.