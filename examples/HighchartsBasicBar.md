Highcharts Basic Bar
====================

Code
----

```fsharp
let basicBar =
    let sales =
        ["2010", 1300; "2011", 1470; "2012", 840; "2013", 1330]
        |> Series.Bar
        |> Series.SetName "Sales"
    let expenses =
        ["2010", 1000; "2011", 1170; "2012", 580; "2013", 1030]
        |> Series.Bar
        |> Series.SetName "Expenses"
    Highcharts.Bar [sales; expenses]

basicBar.ShowLegend()
basicBar.SetTitle "Company Performance"
```
Chart
-----

![Highcharts Basic Bar](https://raw.github.com/TahaHachana/FsPlot/master/screenshots/HighchartsBasicBar.PNG)