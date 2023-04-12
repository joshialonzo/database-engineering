# ACID

ACID: Atomicity, Consistency, Isolation, Durability

Database transaction: It is a collection of queries that are treated as a single unit of work.

* A collection of queries.
* One unit of work.
* Transaction lifespan:
    * Transaction BEGIN
    * Transaction COMMIT
    * Transaction ROLLBACK
* Usually transactions are made to change and modify data.
* Example: Send $100 from account 1 to account 2
    * BEGIN TX1
    * SELECT balance FROM account WHERE id = 1
    * IF balance > 100:
        UPDATE account SET balance = balance - 100 WHERE id = 1
        UPDATE account SET balance = balance + 100 WHERE id = 2
    * COMMIT TX1
* We always use a transaction but this type is manually handled by us, meanwhile, the default ones are handled automatically.

Atomicity:

Isolation:

Consistency:

Durability: