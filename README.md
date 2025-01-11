# Incorrect Usage of $inc Operator in MongoDB Update Query

This repository demonstrates an uncommon error related to the `$inc` operator in MongoDB update queries.  The error arises from providing a string value to the `$inc` operator, which is designed to increment a numeric field.  This leads to unexpected behavior and incorrect data modification.

## Problem Description

The `$inc` operator is intended for incrementing numeric fields in MongoDB documents.  Providing a string value instead of a number results in the operator failing to increment the field correctly.  This can lead to subtle bugs that are difficult to track down.

## Solution

Ensure that the value provided to the `$inc` operator is a number (integer or double).  Avoid passing strings.