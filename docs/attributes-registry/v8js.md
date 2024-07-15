<!--- Hugo front matter used to generate the website version of this page:
--->

<!-- NOTE: THIS FILE IS AUTOGENERATED. DO NOT EDIT BY HAND. -->
<!-- see templates/registry/markdown/attribute_namespace.md.j2 -->

# V8js

## V8 JS Attributes

Describes V8 JS Engine Runtime related attributes.

| Attribute              | Type   | Description                                    | Examples                               | Stability                                                        |
| ---------------------- | ------ | ---------------------------------------------- | -------------------------------------- | ---------------------------------------------------------------- |
| `v8js.gc.type`         | string | The type of garbage collection.                | `major`; `minor`; `incremental`        | ![Experimental](https://img.shields.io/badge/-experimental-blue) |
| `v8js.heap.space.name` | string | The name of the space type of heap memory. [1] | `new_space`; `old_space`; `code_space` | ![Experimental](https://img.shields.io/badge/-experimental-blue) |

**[1]:** Value can be retrieved from value `space_name` of [`v8.getHeapSpaceStatistics()`](https://nodejs.org/api/v8.html#v8getheapspacestatistics)

`v8js.gc.type` has the following list of well-known values. If one of them applies, then the respective value MUST be used; otherwise, a custom value MAY be used.

| Value         | Description                              | Stability                                                        |
| ------------- | ---------------------------------------- | ---------------------------------------------------------------- |
| `incremental` | Incremental (Incremental Marking).       | ![Experimental](https://img.shields.io/badge/-experimental-blue) |
| `major`       | Major (Mark Sweep Compact).              | ![Experimental](https://img.shields.io/badge/-experimental-blue) |
| `minor`       | Minor (Scavenge).                        | ![Experimental](https://img.shields.io/badge/-experimental-blue) |
| `weakcb`      | Weak Callbacks (Process Weak Callbacks). | ![Experimental](https://img.shields.io/badge/-experimental-blue) |

`v8js.heap.space.name` has the following list of well-known values. If one of them applies, then the respective value MUST be used; otherwise, a custom value MAY be used.

| Value                | Description                | Stability                                                        |
| -------------------- | -------------------------- | ---------------------------------------------------------------- |
| `code_space`         | Code memory space.         | ![Experimental](https://img.shields.io/badge/-experimental-blue) |
| `large_object_space` | Large object memory space. | ![Experimental](https://img.shields.io/badge/-experimental-blue) |
| `map_space`          | Map memory space.          | ![Experimental](https://img.shields.io/badge/-experimental-blue) |
| `new_space`          | New memory space.          | ![Experimental](https://img.shields.io/badge/-experimental-blue) |
| `old_space`          | Old memory space.          | ![Experimental](https://img.shields.io/badge/-experimental-blue) |