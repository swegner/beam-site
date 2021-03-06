---
layout: section
title: "Beam SQL: Data Types"
section_menu: section-menu/sdks.html
permalink: /documentation/dsls/sql/data-types/
---

# Beam SQL Data Types

Beam SQL supports standard SQL scalar data types as well as extensions
including arrays, maps, and nested rows. 

In Beam Java, these types are mapped to Java types large enough to hold the
full range of values.

| SQL Type  | Description  | Java class |
| --------- | ------------ | ---------- |
| TINYINT   | 1 byte signed integer in range -128 to 127                                 | java.lang.Byte    |
| SMALLINT  | 2 byte signed integer in range -32768 to 32767                             | java.lang.Short   |
| INTEGER   | 4 byte signed integer in range -2147483648 to 2147483647                   | java.lang.Integer |
| BIGINT    | 8 byte signed integer in range -9223372036854775808 to 9223372036854775807 | java.lang.Long    |
| FLOAT     | 4 byte floating point                                     | java.lang.Float  |
| DOUBLE    | 8 byte floating point                                     | java.lang.Double |
| DECIMAL   | Arbitrary precision decimal value | java.math.BigDecimal     |
| VARCHAR   | Arbitrary length string           | java.lang.String         |
| TIMESTAMP | Millisecond precision timestamp   | org.joda.ReadableInstant |
| ARRAY<type>     | Ordered list of values      | java.util.List |
| MAP<type, type> | Finite unordered map        | java.util.Map  |
| ROW<fields>     | Nested row                  | org.apache.beam.sdk.values.Row |
{:.table}

See also the [documentation for Calcite SQL's data
types](http://calcite.apache.org/docs/reference.html#data-types)
