These are examples of what ee-outliers models for beaconing can look like. These examples are only functional if your data uses the same field names, and if you add the hour and day fields using Logstash. E.g.:
```
"[event][hour_of_day]" => "%{+HH}"
"[event][day_of_month]" => "%{+dd}"
```
You may be able to use derived fields in ee-outliers instead. 