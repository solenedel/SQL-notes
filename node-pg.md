# Connecting to a PG database with node

Install node postgres library: `npm i pg`

In the main server file: 
```
// PG database client/connection setup
const { Pool } = require('pg');
const dbParams = require('./helpers/db-params');
```