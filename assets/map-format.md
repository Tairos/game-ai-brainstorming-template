# HTML map data

Copy `map.html` to the desired output location and populate the JSON in `<script id="map-data" type="application/json">`. The asset works offline; it does not watch files. Serialize JSON and escape `<` as `\u003c` to keep text from terminating the script element.

```json
{
  "id": "spark-tree",
  "title": "Spark branches",
  "premise": "A city that dreams.",
  "ideas": [
    {
      "id": "S1",
      "title": "A city that dreams.",
      "kind": "spark",
      "status": "exploring",
      "summary": "A city that dreams.",
      "parents": [],
      "file": "",
      "feedback": []
    }
  ]
}
```

Use unique IDs and existing parent IDs; do not create cycles. Multiple parents represent a combination. For sparks, title and summary can contain the same one-liner. `kind` identifies maturity (`spark`, `concept`, `direction`, or `blueprint`); `status` separately records disposition (`exploring`, `selected`, `parked`, or `rejected`). User choices determine selection, parking, or rejection.

`file` is optional in practice: use an empty string when no Markdown file exists. The existing map renderer displays a link only for paths matching `ideas/idea-NNN.md`; do not invent files to populate this field. Feedback entries contain `text` and `attribution` strings. Keep them empty unless feedback has actually been given for that idea.

Check IDs, parent relationships, one-liners, and any file links against the source material. Preserve existing branches when extending a map. The map is a read-only view, not a decision-making interface.
