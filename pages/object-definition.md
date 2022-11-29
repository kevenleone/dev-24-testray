---
title: Object Definition
---

# Object Definition

Example of Testray Project Object definition

<div grid="~ cols-2 gap-4">

<div>

```json {all|2-4|5|6-16|17-19|20|all} 
{
	"label": {
		"en_US": "Testray Project"
	},
	"name": "Project",
	"objectFields": [
		{
			"indexed": true,
			"label": {
				"en_US": "Name"
			},
			"name": "name",
			"required": true,
			"type": "String"
		}
	],
	"pluralLabel": {
		"en_US": "Testray Projects"
	},
	"scope": "company",
}
```

</div>

<div>
  <span v-click="1">

  - Object Definition Friendly Name

  </span>

  <span v-click="2">

  - Object Name Friendly Name

  </span>

  <span v-click="3">

  - This array can be used to map all **columns** used in Object Definition, in this case we are mapping the name as ```string, indexable and required```.

  </span>

  <span v-click="4">

  - Same as 2 but Pluralized

  </span>

  <span v-click="5">

  - Scope can be "Site" | "Company"
    - Site scopes the data by the current site that you are accessing, you must pass the siteId to the request, if you have multiple sites, you cannot read from other.
    - Company scopes means that, all sites inside this company can share the data. 

  </span>
</div>

</div>

[^1]: [Learn More](https://sli.dev/guide/syntax.html#line-highlighting)

<style>
.footnotes-sep {
  @apply mt-20 opacity-10;
}
.footnotes {
  @apply text-sm opacity-75;
}
.footnote-backref {
  display: none;
}
</style>

