# Dependency Check Action

This action performs a dependency check, converts the report to Markdown, and adds it to the summary.

## Inputs

| Name             | Description                             | Default                             |
|------------------|-----------------------------------------|-------------------------------------|
| `project_name`   | The name of the project file            | `true`                              |
| `path`           | The path to the project                 | `./`                                |
| `html_report_path` | Path to the HTML report file          | `reports/dependency-check-report.html` |
| `md_report_path` | Path to the Markdown report file        | `dependency-check-report.md`        |

## Example usage

```yaml
uses: yourusername/dependency-check-action@v1
with:
  project_name: 'iPractice.Api.csproj'
  path: './iPractice.Api/'
  html_report_path: 'reports/dependency-check-report.html'
  md_report_path: 'dependency-check-report.md'
