# Methods vs Computed Properties vs Watchers

| Methods      | Computed   | Watch      |
|--------------|-----------|------------|
| For event binding or data binding | For data binding | Not used in template |
| Data binding: Method is executed for every "re-render" cycle of the component | Computed properties are *only re-evaluated* if one of their "used values" changed | Runs any code in *reaction to some changed data* (e.g. send HTTP request etc.) |
| For events or data that really needs to be re-evaluated all the time | Use for data that depends on other data | Use for any non-data update you want to make |
