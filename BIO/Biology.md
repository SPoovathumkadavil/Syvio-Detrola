---
alias: "Biology"
subject: "Science"
subset: "Biology"
importance: 10
type: "Course"
---

> [!info]- What is Biology?
_Biology is the scientific study of life. It is a natural science with a broad scope but has several unifying themes that tie it together as a single, coherent field._

# AP Units
```dataview
LIST
FROM "BIO/AP"
SORT order
```
# 0 - Prevegen Example Report
```dataview
LIST
FROM "BIO/Prevegen Example"
WHERE type = "Guideline"
```
>[!tip]- Prevegen Concepts
>>```dataview
>>TABLE importance
>>FROM "BIO/Prevegen Example"
>>WHERE type = "Concept"
>>SORT 
>>```

# 1 - Measuring Variation within a Population and Sample
```dataview
LIST
FROM "BIO/Measuring Variation within a Population and Sample"
WHERE type="Example" OR type="Guideline" OR type="Bearing"
SORT order
```
>[!tip]- Variation Concepts
>>```dataview
>>TABLE importance
>>FROM "BIO/Measuring Variation within a Population and Sample"
>>WHERE type="Concept"
>>SORT importance DESC
>>```
