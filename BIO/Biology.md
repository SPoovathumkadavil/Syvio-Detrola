---
alias: "Biology"
subject: "Science"
subset: "Biology"
importance: 10
type: "Course"
---
> [!info]- What is Biology?
_Biology is the scientific study of life. It is a natural science with a broad scope but has several unifying themes that tie it together as a single, coherent field._

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
>>SORT importance DESC
>>```

# 1 - Measuring Variation within a Population and Sample
```dataview
LIST
FROM "BIO/Measuring Variation within a Population and Sample"
WHERE type="Example" OR type="Guideline" OR type="Bearing" OR type="Lab"
SORT order
```
>[!tip]- Variation Concepts
>>```dataview
>>TABLE importance
>>FROM "BIO/Measuring Variation within a Population and Sample"
>>WHERE type="Concept"
>>SORT importance DESC
>>```

# 2 - Cell Structure and Function
```dataview
LIST
FROM "BIO/Cell Structure and Function"
WHERE type="Bearing" OR type="Guideline" OR type="Example" OR type="Lab"
SORT order
```
> [!tip]- Structure and Function Concepts
>> ```dataview
>> TABLE importance
>> FROM "BIO/Cell Structure and Function"
>> WHERE type = "Concept"
>> SORT importance DESC
>>```

> [!example]- Structure and Function Artifacts
> >```dataview
> >TABLE importance
> >FROM "BIO/Cell Structure and Function"
> >WHERE type = "Artifact"
> >SORT importance DESC
>>```

# 3 - Expanding on Natural Selection
```dataview
LIST
FROM "BIO/Expanding on Natural Selection"
WHERE type="Bearing" OR type="Guideline" OR type="Example" OR type="Lab"
SORT order
```
> [!tip]- Structure and Function Concepts
>> ```dataview
>> TABLE importance
>> FROM "BIO/Expanding on Natural Selection"
>> WHERE type = "Concept"
>> SORT importance DESC
>>```

> [!example]- Structure and Function Artifacts
> >```dataview
> >TABLE importance
> >FROM "BIO/Expanding on Natural Selection"
> >WHERE type = "Artifact"
> >SORT importance DESC
>>```

## 4 - Quantifying Evolution
```dataview
TABLE importance
FROM "Bio/Quantifying Evolution"
```

## 5 - Community Ecology