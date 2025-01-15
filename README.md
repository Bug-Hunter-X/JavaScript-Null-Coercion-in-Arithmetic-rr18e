# JavaScript Null Coercion Bug

This repository demonstrates a subtle bug in JavaScript related to null value handling during arithmetic operations.  The `foo` function attempts to gracefully handle null inputs by returning 0, but there's an important consideration regarding type coercion.

## Bug Description

The issue arises from JavaScript's loose typing and automatic type coercion.  When a null value is encountered in an addition operation, JavaScript attempts to convert it to a number, resulting in the value 0. This might lead to unexpected results if the intention is to explicitly handle null inputs differently.

## Solution

The solution involves explicitly checking for null values before performing the addition to avoid unintended type coercion.