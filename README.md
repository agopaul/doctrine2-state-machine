# Doctrine 2 State Machine (Work in progress)

## State machines for Doctrine entities

### Why

State machines when used to enforce the workflow of DB records, need to be deeply integrated with the underlying DBMS in order to retain data integrity in a highly concurrency environment.

eg. Suppose you're working on an eCommerce with limited inventory, you wouldn't want to sell the same item to more than one person. That is why a state machine should adopt a locking strategy on the DB in order to prevent double state updates on the same record.
