# Camel-JMS-JDBC demo

Tested against JBoss Fuse 6.0 (RC1).

A Camel based demo that shows how route messages through JMS and JDBC.
Access to an external JDBC database is needed to run this demo.
The demo currently connects to a local PostgreSQL instance but can be easily 
reconfigured to work with any other JDBC database.

The demo defines two similar Camel routes. However one route uses the 
camel-sql component, the other route uses the camel-jdbc component. 
Both routes consume messages from a JMS destination, then call the JDBC database
and finally send the message to another JMS destination.



