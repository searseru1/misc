# loki

### Query examples
```
count_over_time({system="AD"} |~ "4624" |~ "SuccessAudit" !~ "ERR|err|Err" [5m])
{system="id"} |~ "Logon Type:.*3" | json | EventID="4634"
```