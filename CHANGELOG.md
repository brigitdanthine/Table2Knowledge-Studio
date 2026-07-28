# V2.0.0
- The application has been renamed from **Table2Knowledge Studio** to **OntoCartographer Studio**. Existing project files continue to load unchanged; only the name and the documentation are affected.
- Custom Explorer names can now be assigned to nodes and connections. Such a name replaces the ontology class or property name in the GraphExplorer view, and connections sharing the same Explorer name are merged into a single group there. Explorer names are used exclusively in the JSON export and leave the RDF export unchanged.
- A JSON export for the GraphExplorer has been added. Free-text values that had to be modelled as separate nodes on the canvas (e.g. a note attached via `P3_has_note`) are folded into the attributes of their parent node instead of being exported as standalone nodes. The GraphExplorer itself is not published yet.
- The inverse of a connection can now be controlled manually: an inverse property URI can be entered where the loaded ontology declares no `owl:inverseOf` or where a custom property is used, and the creation of the inverse relation can be switched off per connection.

# V1.1.0
- Key handling has been improved: instead of a single join key, it is now possible to select separate join keys for domain (source) and range (target), ensuring correct cross-table joins.
- A new widening function has been added: it is now possible to separately activate or deactivate widening for parent properties (properties inherited from parent entities) and child properties (properties defined on child entities).
