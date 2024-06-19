# Dependency Check Action

This action performs a dependency check, uploads it as an artifact and optionally converts the report to Markdown, and adds it to the summary.

## Inputs

| Name             | Description                             | Default                             |
|------------------|-----------------------------------------|-------------------------------------|
| `project_name`   | The name of the project file            |                                     |
| `path`           | The path to the project                 | `./`                                |
| `html_report_path` | Path to the HTML report file          | `reports/dependency-check-report.html` |
| `md_report_path` | Path to the Markdown report file        | `dependency-check-report.md`        |
| `md_report_path` | Whether to add the report to the summary        | `false`        |

## Example usage

```yaml
uses: KKica/dependency-check-action@v0.1.0
with:
  project_name: 'iPractice.Api.csproj'
  path: './iPractice.Api/'
  html_report_path: 'reports/dependency-check-report.html'
  md_report_path: 'dependency-check-report.md'
  add_report_to_summary: 'true'
