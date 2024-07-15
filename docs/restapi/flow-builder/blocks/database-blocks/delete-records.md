---
sidebar_position: 4
title: 'Delete Records'
description: Learn to about Delete Records! 
sidebar_label: Delete Records
---

# Delete Records

The DeleteOne and DeleteMany blocks in Zeromagic facilitate the removal of data from a Cosmos DB container. These blocks offer the capability to delete either a single record or multiple records from your database.


## 1. Delete One

Deletes a single record by its ID from a Cosmos DB container.

### Properties

**Container Name**: The name of the Cosmos DB container from which the record will be deleted.

**Record ID**: The unique identifier of the record to be deleted.

**Returns**: Return a `val` with the ID of deleted record.

## 2. Delete Many

Deletes multiple records based on a filter query from a Cosmos DB container.

### Properties

**Container Name**: The name of the Cosmos DB container from which the records will be deleted.

**Filter Query**: A filter query used to identify the records to be deleted. The filter query consists of a left value `(field name)` and a right value `(data to be evaluated)`.

**Returns**: Return a `val` with the IDs of deleted records.

It utilises the same condition syntax as the [If Conditions](/flow-builder/blocks/flow-control/if-else#condition-editor).


:::warning Return Value

Delete records does not return any value.

:::