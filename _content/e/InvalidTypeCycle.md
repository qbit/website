---
title: InvalidTypeCycle
layout: article
---
<!-- Copyright 2023 The Go Authors. All rights reserved.
     Use of this source code is governed by a BSD-style
     license that can be found in the LICENSE file. -->

<!-- Code generated by generrordocs.go; DO NOT EDIT. -->

```
InvalidTypeCycle occurs when a cycle in type definitions results in a
type that is not well-defined.

Example:
 import "unsafe"

 type T [unsafe.Sizeof(T{})]int
```
