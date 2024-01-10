file:: [rfc8610.txt_1703631168898_0.pdf](../assets/rfc8610.txt_1703631168898_0.pdf)
file-path:: ../assets/rfc8610.txt_1703631168898_0.pdf

- The CBOR notational convention has the following goals:
  ls-type:: annotation
  hl-page:: 4
  hl-color:: blue
  id:: 658b5c6d-9f29-4654-bf0c-f3c3f692858b
- Not an original goal per se, but a convenient side effect of the JSON generic data model being a subset of the CBOR generic data model, is the fact that CDDL can also be used for describing JSON data structures (see Appendix E).
  ls-type:: annotation
  hl-page:: 4
  hl-color:: blue
  id:: 658b5c83-8524-40b1-a55f-da49f4b0f1be
- CDDL focuses on styles of specification that are in use in the community employing the data model as pioneered by JSON and now refined in CBOR.
  ls-type:: annotation
  hl-page:: 5
  hl-color:: blue
  id:: 658b5df2-a104-4197-a4b2-c476b6a76fdf
- There are a number of more or less atomic elements of a CBOR data model, such as numbers, simple values (false, true, nil), text strings, and byte strings; CDDL does not focus on specifying their structure.
  ls-type:: annotation
  hl-page:: 5
  hl-color:: blue
  id:: 658b5e2b-1ea3-4ffe-8cae-f92b52e456c9
- Beyond those atomic elements, further components of a data structure definition language are the datatypes used for composition:
  ls-type:: annotation
  hl-page:: 5
  hl-color:: blue
  id:: 658b5e45-8771-43e6-be8d-3e925945f2a2
- Two important concepts provide the foundation for CDDL:
  ls-type:: annotation
  hl-page:: 6
  hl-color:: blue
  id:: 658b5e65-9309-482d-a3a2-237e7bbdd191
- Instead of defining all four types of composition in CDDL separately, or even defining one kind for arrays (vectors and records) and one kind for maps (tables and structs), there is only one kind of composition in CDDL: the _group_ (Section 2.1).
  ls-type:: annotation
  hl-page:: 6
  hl-color:: blue
  id:: 658b5e6e-ba85-4722-af15-96b69719ebab
- The other important concept is that of a _type_. The entire CDDL specification defines a type (the one defined by its first _rule_), which formally is the set of CBOR data items that are acceptable as "instances" for this specification. CDDL predefines a number of basic types such as "uint" (unsigned integer) or "tstr" (text string), often making use of a simple formal notation for CBOR data items. Each value that can be expressed as a CBOR data item is also a type in its own right, e.g., "1". A type can be built as a _choice_ of other types, e.g., an "int" is either a "uint" or a "nint" (negative integer). Finally, a type can be built as an array or a map from a group.
  ls-type:: annotation
  hl-page:: 6
  hl-color:: blue
  id:: 658b5e94-b99b-4b06-88db-cef2e5219b89
- CDDL groups are lists of group _entries_, each of which can be a name/value pair or a more complex group expression (which then in turn stands for a sequence of name/value pairs).
  ls-type:: annotation
  hl-page:: 7
  hl-color:: blue
  id:: 658b61f2-a1f2-4934-8ec1-21f83539f784
- In an array context, only the value of the name/value pair is represented; the name is annotation only (and can be left off from the group specification if not needed).
  ls-type:: annotation
  hl-page:: 7
  hl-color:: blue
  id:: 658b6214-1e55-4b72-a35c-50e8280b851b
- In a map context, the names become the map keys ("member keys").
  ls-type:: annotation
  hl-page:: 7
  hl-color:: blue
  id:: 658b6220-5f19-4837-ba04-f0718d4fb366
- In an array context, the actual sequence of elements in the group is important, as that sequence is the information that allows associating actual array elements with entries in the group.
  ls-type:: annotation
  hl-page:: 7
  hl-color:: blue
  id:: 658b622c-4e04-4153-af0c-642b289114f0
- A group by itself (without creating a map around it) can be placed in(round) parentheses and given a name by using it in a rule
  ls-type:: annotation
  hl-page:: 8
  hl-color:: blue
  id:: 658b62d4-3912-4e7a-9e82-a19e5873ce29
- Note that the (curly) braces signify the creation of a map; the groups themselves are neutral as to whether they will be used in a map or an array.
  ls-type:: annotation
  hl-page:: 8
  hl-color:: blue
  id:: 658b646d-671f-4c57-8dff-5a8ab82de625
- Groups can be used to factor out common parts of structs, e.g., instead of writing specifications in copy/paste style
  ls-type:: annotation
  hl-page:: 9
  hl-color:: blue
  id:: 658b6664-2eff-47f4-9b1d-9f4e4600d76e
- Groups are the instrument used in composing data structures with CDDL. It is a matter of style in defining those structures whether to define groups (anonymously) right in their contexts or whether to define them in a separate rule and to reference them with their respective name (possibly more than once).
  ls-type:: annotation
  hl-page:: 10
  hl-color:: blue
  id:: 658b667a-2f4c-4e86-bdd6-87329ea36bb8
- A basic entry consists of a _keytype_ and a _valuetype_, both of which are types (Section 2.2); this entry matches any name/value pair the name of which is in the keytype and the value of which is in the valuetype.
  ls-type:: annotation
  hl-page:: 10
  hl-color:: blue
  id:: 658b67a9-a142-4d89-b4fa-aac0acf76028
- Values such as numbers and strings can be used in place of a type.
  ls-type:: annotation
  hl-page:: 11
  hl-color:: blue
  id:: 658b67be-c2b3-49b6-9d7e-0e1d6d9c69fd
- The value notation for numbers inherits from C the distinction between integer values (no fractional part or exponent given -- NR1 [ISO6093];"NR" stands for "numerical representation") and floating-point values(where a fractional part, an exponent, or both are present -- NR2 or NR3), so the type "1" does not include any floating-point numbers while the types "1e3" and "1.5" are both floating-point numbers and do not include any integer numbers.
  ls-type:: annotation
  hl-page:: 11
  hl-color:: blue
  id:: 658b67eb-f1d0-4881-8735-74c2c214e807
- Many places that allow a type also allow a choice between types, delimited by a "/" (slash).
  ls-type:: annotation
  hl-page:: 11
  hl-color:: blue
  id:: 658b6803-f39f-49d7-ba2d-d31b30967142
- Analogous to types, CDDL also allows choices between groups, delimited by a "//" (double slash). Note that the "//" operator binds much more weakly than the other CDDL operators, so each line within "delivery" in the following example is its own alternative in the group choice
  ls-type:: annotation
  hl-page:: 11
  hl-color:: blue
  id:: 658b681b-5860-4ab6-b174-26158a18cd9d
- Instead of naming all the values that make up a choice, CDDL allows building a _range_ out of two values that are in an ordering relationship: a lower bound (first value) and an upper bound (second value). 
  ls-type:: annotation
  hl-page:: 12
  hl-color:: blue
  id:: 658b684d-43f5-43b7-ac80-506925262bc7
- When using a name as the left-hand side of a range operator, use spacing as in min .. max to separate off the range operator.
  ls-type:: annotation
  hl-page:: 13
  hl-color:: blue
  id:: 658b6874-c5ad-4391-9cee-15887250cef8
- CDDL allows the specification of a data item type by referring to the CBOR representation (specifically, to major types and additional information; see Section 2 of [RFC7049]). How this is used should be evident from the prelude (Appendix D): a hash mark ("#") optionally followed by a number from 0 to 7 identifying the major type, which then can be followed by a dot and a number specifying the additional information.
  ls-type:: annotation
  hl-page:: 13
  hl-color:: blue
  id:: 658b69dd-1719-4d43-bca6-723c303b270b
- It may be necessary to make use of representation types outside the prelude, e.g., a specification could start by making use of an existing tag in a more specific way or could define a new tag not defined in the prelude:
  ls-type:: annotation
  hl-page:: 14
  hl-color:: blue
  id:: 658b6a13-579e-49a0-82d8-99396c6b7151
- There is no special syntax to identify the root of a CDDL data structure definition: that role is simply taken by the first rule defined in the file.
  ls-type:: annotation
  hl-page:: 14
  hl-color:: blue
  id:: 658b6c73-7664-42c5-b14e-cb16f7082792
- (Note that there is no way to use a group as a root -- it must be a type.)
  ls-type:: annotation
  hl-page:: 14
  hl-color:: blue
  id:: 658b6c82-17b6-4e86-b995-48d6aa425abd