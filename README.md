# PartiaViewMVC

PARTIAL VIEWS IN ASP.NET MVC
•	Partial view represents a sub-view of a main view.
•	Partial view allows you to reuse common markups across the different views of the application.
•	We can use partial views in different views.
•	Partial views cannot be used separately, we have to attach partial in some other view.
•	Partial view extension is .cshtml like a view.
•	When we have to use some html markup on some pages not all pages then we can use partial view.
To create a partial view in Visual Studio .NET, you need to perform the following steps:
1.	Right-click the Views/Shared folder in the Solution Explorer window and select Add View. The AddView dialog box is displayed.
2.	In the AddView dialog box, specify a name for the partial view in the View Name text field.
3.	Select the Create as a partial view check box.
There are 2 types of partial views.
1.	Static
a.	Views whose layout not changed i.e header, footer, navigation bar etc.
2.	Dynamic
a.	Views whose contents can change accordingly, just like shopping cart where number of product can be changed.
For static partial views we use two methods of html helper class.
1.	Html.Partial
2.	Html.RenderPartial
For dynamic partial views we use two methods of html helper class.
3.	Html.Action
4.	Html.RenderAction
SIMILARITIES AND DIFFERENCE BETWEEN HTML.PARTIAL AND HTML.RENDERPARTIAL
•	Both Html.Partial and Html.RenderPartial can be used to access or display a partial view in a view
Html.Partial	Html.RenderPartial
Method that returns MVCHtmlString	Method without any return value, it means it returns void.
Rendered Partial view result can be stored in string variable.	Rendered Partial view result cannot be stored in string variable.
Slow in access	Fast in access
