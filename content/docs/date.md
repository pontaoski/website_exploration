---
title: date
layout: command
nu_version: 0.14
---

Use `date` to get the current date and time. Defaults to local timezone but you can get it in UTC too.

## Flags

{{< flag "" "utc" >}}
Returns the current date and time in UTC
{{< /flag >}}
{{< flag "" "local" >}}
Returns the current date and time in your local timezone
{{< /flag >}}

## Examples

```shell
> date
━━━━━━┯━━━━━━━┯━━━━━┯━━━━━━┯━━━━━━━━┯━━━━━━━━┯━━━━━━━━━━
 year │ month │ day │ hour │ minute │ second │ timezone
──────┼───────┼─────┼──────┼────────┼────────┼──────────
 2019 │     9 │  30 │   21 │     52 │     30 │ -03:00
━━━━━━┷━━━━━━━┷━━━━━┷━━━━━━┷━━━━━━━━┷━━━━━━━━┷━━━━━━━━━━
> date --utc
━━━━━━┯━━━━━━━┯━━━━━┯━━━━━━┯━━━━━━━━┯━━━━━━━━┯━━━━━━━━━━
 year │ month │ day │ hour │ minute │ second │ timezone
──────┼───────┼─────┼──────┼────────┼────────┼──────────
 2019 │    10 │   1 │    0 │     52 │     32 │ UTC
━━━━━━┷━━━━━━━┷━━━━━┷━━━━━━┷━━━━━━━━┷━━━━━━━━┷━━━━━━━━━━
> date --local
━━━━━━┯━━━━━━━┯━━━━━┯━━━━━━┯━━━━━━━━┯━━━━━━━━┯━━━━━━━━━━
 year │ month │ day │ hour │ minute │ second │ timezone
──────┼───────┼─────┼──────┼────────┼────────┼──────────
 2019 │     9 │  30 │   21 │     52 │     34 │ -03:00
━━━━━━┷━━━━━━━┷━━━━━┷━━━━━━┷━━━━━━━━┷━━━━━━━━┷━━━━━━━━━━
```
