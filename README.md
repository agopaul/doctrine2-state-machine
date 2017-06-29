# Doctrine 2 State Machine

## State machines for Doctrine entities

### Why

State machines when applied to DB records, needs to be deeply integrated with the underlying DBMS in order to retain data integrity in a highly concurrency environment.
Ie. Suppose you're working on an eCommerce with limited inventory, you wouldn't want to sell the same item to more than one person. That is why a state machine should adopt a locking strategy on the DB in order to prevent double state updates on the same record. 
