# How-to-change-the-bubble-color-on-the-cursor-hover-in-bubble-series

This article explains how to change the bubble color on the cursor hover in Blazor chart component.

**Highlighting bubble point on mouse hover**

[Blazor Chart](https://www.syncfusion.com/blazor-components/blazor-charts) provides support to change color of the Bubble points on mouse hover by using highlight color and highlight mode property.

The color which needs to be changes is set to the [HighLightColor](https://help.syncfusion.com/cr/blazor/Syncfusion.Blazor.Charts.SfChart.html#Syncfusion_Blazor_Charts_SfChart_HighlightColor) property and the [HighLightMode](https://help.syncfusion.com/cr/blazor/Syncfusion.Blazor.Charts.SfChart.html#Syncfusion_Blazor_Charts_SfChart_HighlightMode) is set to **Point**.

The following code snippet illustrates this.

**C#**

```cshtml

@using Syncfusion.Blazor.Charts

<SfChart HighlightColor="red" HighlightMode="HighlightMode.Point">
    <ChartSeriesCollection>
        <ChartSeries DataSource="@SalesReports" XName="X" YName="Y" Type="ChartSeriesType.Bubble">
        </ChartSeries>
    </ChartSeriesCollection>
</SfChart>

@code {

    public class ChartData
    {
        public double X { get; set; }
        public double Y { get; set; }
        public string Text { get; set; }
    }

    public List<ChartData> SalesReports = new List<ChartData>
    {
        new ChartData { X= 92.2, Y= 7.8, Text= "China" },
        new ChartData { X= 74, Y= 6.5, Text= "India" },
        new ChartData { X= 90.4, Y= 6.0, Text= "Indonesia" },
        new ChartData { X= 99.4, Y= 2.2, Text= "US" },
        new ChartData { X= 88.6, Y= 1.3, Text= "Brazil" },
        new ChartData { X= 99, Y= 0.7, Text= "Germany" },
        new ChartData { X= 72, Y= 2.0, Text= "Egypt" },
        new ChartData { X= 99.6, Y= 3.4, Text= "Russia" },
        new ChartData { X= 99, Y= 0.2, Text= "Japan" },
        new ChartData { X= 86.1, Y= 4.0, Text= "Mexico" },
        new ChartData { X= 92.6, Y= 6.6, Text= "Philippines" },
        new ChartData { X= 61.3, Y= 1.45, Text= "Nigeria" },
        new ChartData { X= 82.2, Y= 3.97, Text= "Hong Kong" },
        new ChartData { X= 79.2, Y= 3.9, Text= "Netherland" },
        new ChartData { X= 72.5, Y= 4.5, Text= "Jordan" },
        new ChartData { X= 81, Y= 3.5, Text= "Australia" },
        new ChartData { X= 66.8, Y= 3.9, Text= "Mongolia" },
        new ChartData { X= 78.4, Y= 2.9, Text= "Taiwan" }
    };
}

```

The following image screenshot illustrate this.

**Output:**

![](/bubble-point-color-change-on-hover.png)

**Conclusion**

I hope you enjoyed learning how to change bubble color on cursor hover in Blazor Chart Component.

You can refer to our [Blazor Chart feature tour](https://www.syncfusion.com/blazor-components/blazor-charts) page to know about its other groundbreaking feature representations and [documentation](https://blazor.syncfusion.com/documentation/chart/getting-started), and how to quickly get started for configuration specifications. You can also explore our [Blazor Chart example](https://blazor.syncfusion.com/demos/chart/line?theme=bootstrap5) to understand how to create and manipulate data.

For current customers, you can check out our components from the [License and Downloads](https://www.syncfusion.com/sales/teamlicense) page. If you are new to Syncfusion, you can try our 30-day [free trial](https://www.syncfusion.com/downloads/blazor) to check out our other controls.

If you have any queries or require clarifications, please let us know in the comments section below. You can also contact us through our [support forums](https://www.syncfusion.com/forums), [support portal](https://support.syncfusion.com/create), or [feedback portal](https://www.syncfusion.com/feedback/blazor-components?control=charts). We are always happy to assist you!
