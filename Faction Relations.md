---
BuildersReputation: "-4"
CelebrantsReputation: "4"
ReanimatorsReputation: "10"
ExportRelations: "4"
SecretPoliceReputation: "0"
TaxCollectorsGuildReputation: "8"
---
# Graph:

```dataviewjs
const data = dv.current()

const chartData = {
    type: 'bar',
    data: {
        labels: ["Builders League", "Celebrants", "Export Guild", "Tax Collector's Union", "Reanimators"],
        datasets: [{
            label: 'Reputation',
            data: [data.BuildersReputation, data.CelebrantsReputation, data.ExportRelations, data.TaxCollectorsGuildReputation, data.ReanimatorsReputation],
            backgroundColor: [
                'rgba(255, 99, 132, 0.2)'
            ],
            borderColor: [
                'rgba(255, 99, 132, 1)'
            ],
            borderWidth: 1
        }]
    }
}

window.renderChart(chartData, this.container);
```

# Reanimators

| Event                    | Modifier |
| ------------------------ | -------- |
| Starting level           | 0        |
| Clearing Berline's Farm: | 5        |
| Debt for  Emeritus       | 3        |
| Berline's Thoughts       | 2        |
| Total:                   | 10       |
<!-- TBLFM: @>$2=sum(@I..@-1) -->

# Builder's League

| Event                                        | Modifier |
| -------------------------------------------- | -------- |
| Starting level                               | 0        |
| Left the bank with the Tax Collector's union | -4       |
| Total:                                       | -4       |
<!-- TBLFM: @>$2=sum(@I..@-1) -->
# Celebrants 

| Event                           | Modifier |
| ------------------------------- | -------- |
| Starting level                  | 0        |
| Se-Maut-Get Rescue from Kepgeda | 4        |
| Total:                          | 4        |
<!-- TBLFM: @>$2=sum(@I..@-1) -->
# Export Guild

| Event          | Modifier |
| -------------- | -------- |
| Starting level | 0        |
| Altinmered     | 4        |
| Total:         | 4        |
<!-- TBLFM: @>$2=sum(@I..@-1) -->
# Tax Collectors Union

| Event                       | Modifier |
| --------------------------- | -------- |
| Starting level              | 0        |
| Allowed the Bank to re-open | 8        |
| Total:                      | 8        |
<!-- TBLFM: @>$2=sum(@I..@-1) -->
# Secret Police

| Event          | Modifier |
| -------------- | -------- |
| Starting level | 0        |
