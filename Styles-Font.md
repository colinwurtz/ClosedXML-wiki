## Styles - Font

![Styles_Font.jpg](http://download-codeplex.sec.s-msft.com/Download?ProjectName=closedxml&DownloadId=165392 "Styles_Font.jpg")  

```c#
var workbook = new XLWorkbook();
var ws = workbook.Worksheets.Add("Style Font");

var co = 2;
var ro = 1;

ws.Cell(++ro, co).Value = "Bold";
ws.Cell(ro, co).Style.Font.Bold = true;

ws.Cell(++ro, co).Value = "FontColor - Red";
ws.Cell(ro, co).Style.Font.FontColor = XLColor.Red;

ws.Cell(++ro, co).Value = "FontFamilyNumbering - Script";
ws.Cell(ro, co).Style.Font.FontFamilyNumbering = XLFontFamilyNumberingValues.Script;

ws.Cell(++ro, co).Value = "FontName - Stencil";
ws.Cell(ro, co).Style.Font.FontName = "Stencil";

ws.Cell(++ro, co).Value = "FontSize - 15";
ws.Cell(ro, co).Style.Font.FontSize = 15;

ws.Cell(++ro, co).Value = "Italic - true";
ws.Cell(ro, co).Style.Font.Italic = true;

ws.Cell(++ro, co).Value = "Shadow - true";
ws.Cell(ro, co).Style.Font.Shadow = true;

ws.Cell(++ro, co).Value = "Strikethrough - true";
ws.Cell(ro, co).Style.Font.Strikethrough = true;

ws.Cell(++ro, co).Value = "Underline - Double";
ws.Cell(ro, co).Style.Font.Underline = XLFontUnderlineValues.Double;

ws.Cell(++ro, co).Value = "VerticalAlignment = Superscript";
ws.Cell(ro, co).Style.Font.VerticalAlignment = XLFontVerticalTextAlignmentValues.Superscript;

ws.Column(co).AdjustToContents();

workbook.SaveAs("StylesFont.xlsx");
```
