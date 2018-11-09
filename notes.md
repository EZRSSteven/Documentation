[Snippets](https://gist.github.com/EZRSSteven/1f175739108d5eebbcbbfbb1abce4e25)

**GIST NOTES**

### Basic writing and formatting syntax.

`https://help.github.com/articles/basic-writing-and-formatting-syntax/`

###  Creating and highlighting code blocks.

`https://help.github.com/articles/creating-and-highlighting-code-blocks/`

```C#
using System;
using System.Collections.Generic;
using System.Linq;
using System.Web;
using System.Web.UI;
using System.Web.UI.WebControls;

public partial class SpaPackages_JoinWaitingListResult : System.Web.UI.Page
{
    protected void Page_Load(object sender, EventArgs e)
    {
        if (!IsPostBack)
        {
            var waitingListSuccess = Session["WaitingListSuccess"].ToString();

            labelWaitingListSuccess.Text = waitingListSuccess.ToUpper() == "TRUE"
                ? "You have succesfully been added to the waiting list."
                : "There was an issue adding you to the waiting list.";
        }
    }
}
```




