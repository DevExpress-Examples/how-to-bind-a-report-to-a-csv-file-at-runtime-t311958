<!-- default file list -->
*Files to look at*:

* [Form1.cs](./CS/BindingReportToCsvFile/Form1.cs) (VB: [Form1.vb](./VB/BindingReportToCsvFile/Form1.vb))
* [Program.cs](./CS/BindingReportToCsvFile/Program.cs) (VB: [Program.vb](./VB/BindingReportToCsvFile/Program.vb))
<!-- default file list end -->
# How to: Bind a Report to a CSV file at runtime


<p>This code example demonstrates how to create a new blank report at runtime (an instance of the <strong>XtraReport</strong> class), bind it to data obtained from a CSV file, and then, fill the report with a <strong>DetailBand</strong> containing an <strong>XRLabel</strong> to show data from this file.</p>
<p>To bind a report to a CSV file, create a new instance of the <strong>ExcelDataSource</strong> class and specify the full path to the source file using the <strong>FileName</strong> property. Then, specify required settings used to extract data from the file and manually define the data source schema. Finally, assign the created data source to the report using the <strong>DataSource</strong> property.</p>
<p>In this example, an <strong>XRLabel</strong> is added to the report to display data of one data field.<br><br></p>
<p>Starting with v.17.2, the report uses <a href="https://documentation.devexpress.com/XtraReports/119236/Creating-Reports-in-Visual-Studio/Detailed-Guide-to-DevExpress-Reporting/Providing-Data-to-Reports/Data-Binding-Overview/Data-Binding-Modes">expression bindings</a> to provide data to controls. You can switch to the legacy binding mode by setting the <a href="https://documentation.devexpress.com/XtraReports/DevExpress.XtraReports.Configuration.UserDesignerOptions.DataBindingMode.property">UserDesignerOptions.DataBindingMode</a> property to <strong>Bindings </strong>at the application startup.</p>

<br/>


