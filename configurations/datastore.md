# Datastore Configuration Guide for Pebble's CobbledGTS

This guide will help you configure the datastore for Pebble's CobbledGTS, including options for JSON, MongoDB, and MySQL databases.

## Overview

The datastore configuration is crucial for determining where and how the data for the Global Trade System (GTS) is stored and managed. You have the option to choose between a simple JSON file, MongoDB, or MySQL depending on your needs and setup.

## Configuration Files

- **datastore.json**: Main configuration file to select the type of datastore.
- **mongodb.json**: Specific configuration for MongoDB connections.
- **mysql.json**: Specific configuration for MySQL connections.

## Configuring Datastore Type

In `datastore.json`, you will specify the type of datastore you wish to use. The available options are:

- `JSON`: Stores data in a simple JSON file. Good for smaller or test environments.
- `MONGODB`: Utilizes a MongoDB database. Preferred for scalable and production environments.
- `MYSQL`: Utilizes a MySQL database. A common choice for relational database management.

## MongoDB Configuration

To use MongoDB as your datastore, configure the following in `mongodb.json`:

- `connectionString`: The connection string for your MongoDB instance.
- `database`: The name of the database to use.
- `pokemonListingCollection`: The collection name for Pokemon listings.
- `itemListingCollection`: The collection name for item listings.
- `balanceCollection`: The collection name for user balances.

## MySQL Configuration

To use MySQL as your datastore, configure the following in `mysql.json`:

- `connectionString`: The JDBC connection string for your MySQL database.
- `database`: The name of the database to use.
- `pokemonListingTable`: The table name for Pokemon listings.
- `itemListingTable`: The table name for item listings.
- `balanceTable`: The table name for user balances.

## Example Configuration

Here's an example of what your `datastore.json` might look like when using MongoDB:

```json
{
    "datastore": "MONGODB"
}
```