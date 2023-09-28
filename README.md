<%@ Page Language="C#" AutoEventWireup="true" CodeBehind="shoppig card.aspx.cs" Inherits="java.shoppig_card" %>

<!DOCTYPE html>

<html xmlns="http://www.w3.org/1999/xhtml">
<head runat="server">
    <title>GIỎ HÀNG</title>
    <script type="text/javascript">
        function calculate() {
            var dg = parsefloat(window.document.getElementById("dg").value);
            var sl = parsefloat(window.document.getElementById("sl").value);
            window.document.getElementById("tt").value = dg * sl;
        }
    </script>
</head>
<body>
    <form id="form1" runat="server" method="post">
        <div>
            Đơn giá <input type="number" id="dg"value="10000" />
            Số lương <input type="number" id="sl"value=""min="1" max="10"step="1" 
              <%--  onkeyup="tt.value=parsefloat(dg.value)*parsefloat(sl.value);"
                onchange="tt.value=parsefloat(dg.value)*parsefloat(sl.value);"--%>
                />
            Thành tiền <input type="number" id="tt" />
        </div>
    </form>
</body>
</html>
