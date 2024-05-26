# Certification Corrected

- The **PROFILE** keyword executes the query. **EXPLAIN** only provides the plan.

- A node can have a relationship referencing itself or another node.
	- Hence, a relationship can connect one or two nodes

- A relationship connects two nodes — A start-node and an end-node

- Subqueries can be used for post **UNION** processing
	- Neo4j requires all relationships to have a **DIRECTION** and a **TYPE**.
	
- A best practice is to only create one relationship of a given type between two nodes,
	- HOWEVER, you can create the same relationship type between nodes, each with different properties.
	
- Cypher **PROFILE** is used to return the query plan and execution information for a Cypher statement (purpose: Performance tuning)\

- Property Types:
	- String
	- Long (integer values)
	- Double (decimal values)
	- Boolean
	- Date/Datetime
	- Point (spatial)
	- StringArray (comma-separated list of strings)
	- LongArray (comma-separated list of integer values)
	- DoubleArray (comma-separated list of decimal values)
	
- Returns the string representation of the relationship type. The relationship type:
		- (a)-[b]->(c)
		- type(b)
	
- count(*)* returns the number of matching rows.

- **count(n)** returns the number of non- null values returned by an expression.
- Neo4j **does NOT** enforce that all nodes with the same label must have the same property keys.
- Two nodes can be connected **BY MORE THAN 1** relationship
- For querying data from a Neo4j DB, you can use the Bolt protocol and from the Neo4j Browser, you can execute the query statements
- Neo4j Graph Database has the following building blocks −
	1.  Nodes
	2. Properties
	3. Relationships
	4. Labels
	5. Data Browser
- In Browser you can use **CALL db.constraints** to get all constraints on graph.
- CALL db.propertyKeys()
- WHEN SHOULD WE USE BI-DIRECTIONAL RELATIONSHIPS ??
- CALL db.propertyKeys() to see all the keys used in the graph
- If you want to get the labels of a specify node, then use labels(node)
- CONSTRAINTS: Unique node property constraints, or node property **uniqueness constraints**, ensure that property values are unique for all nodes with a specific label
- Site: **graphgists** for modeling examples
- LIMIT : To return a limited subset of the rows