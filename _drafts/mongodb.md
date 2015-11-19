//update()
db.collectionName.update(
		{"name": "Carlos" }, -> Query Parameter
		{"$set": { "city": "NYC" }}, -> Update Parameter
		{"$inc"" {"count": 1} } -> $inc Operator
		{"multi": true } -> Options Parameter,
		{"upsert": true} -> Upsert Option
	)

Update parameters always being with a $ and only updates that field, without the update parameter, the entire document would be replace, except for the ID.

Option Parameter - if set to true, it performs operation on all matching documents. Otherwise, only the first matching document gets updated. 

$inc Operator - increments the count of an existing log document

Upsert - either updates an existing document or creates a new one. It creates a document using the values from the query and update parameter.