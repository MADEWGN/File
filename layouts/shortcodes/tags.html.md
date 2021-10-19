{{- range $name, $taxonomy = (where .Site.Taxonomies.tags "Section" "post") }}
{{- if eq (lower $name) "batch" }}
## true
{{ .Title }}
{{ end -}}
{{ end -}}