# Methods vs Computed Properties vs Watchers

| Methods      | Computed   | Watch      |
|--------------|-----------|------------|
| Use with event binding OR data binding | Use with data binding | Not used directly in template |
| Data binding: Method is executed for every "re-render" cycle of the component | Computed properties are only re-evaluated if one of their "used values" changed | Allows you to run any code in reaction to some changed data (e.g. send HTTP request etc.) |
| Use for events or data that really needs to be re-evaluated all the time | Use for data that depends on other data | Use for any non-data update you want to make |
