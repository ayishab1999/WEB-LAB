# lab 1
 lab program
<!--Javascript calculator to perform
SUM, MUL, DIV, ADD
-->
<!DOCTYPE html>
<html>
<head><title>Lab Pgm 1</title>
    <style>
         .title{
             border-radius: 5px;
             margin-bottom: 10px;
             text-align: center;
             width: 400px;
             color: blue;
             background-color: chartreuse;
             border:solid black 1px;
         }
         input[type="text"]{
             border-radius: 5px;
             text-align: right;
             background-color: white;
             width: 94%;
         }
        input[type="button"]{
            border-radius: 5px;
            background-color:#ff4456;
            color: black;
            border-color: #ff4456;
            width: auto;
        }
    </style>
    <script>
          function disp(val){
              document.getElementById('sdm').value+=val;

          }
          function clr(){
              document.getElementById('sdm').value=" ";
          }

          function solve(){
             let x= document.getElementById('sdm').value;
             let y=eval(x);
             document.getElementById("sdm").value=y
          }
    </script>
</head>
<body>
    <div class="title">SDM --Javascript lab program</div>
<!--Ceate a table-->
 <table border="2">
    <tr>
        <td>
            <input type="button" value="CE" onclick="clr()">
        </td>
        <td colspan="3">
            <input type="text" id="sdm">
        </td>
    </tr>
    <!-- creating buttons and assign values to it-->
    <tr>
        <td>
            <input type="button" value="+" onclick="disp('+')">
        </td>
        <td>
            <input type="button" value="1" onclick="disp('1')" >
        </td>
        <td>
            <input type="button" value="2" onclick="disp('2')">
        </td>
        <td>
            <input type="button" value="3" onclick="disp('3')">
        </td>
    </tr>
    <tr>
        <td>
            <input type="button" value="-" onclick="disp('-')">
        </td>
        <td>
            <input type="button" value="4" onclick="disp('4')">
        </td>
        <td>
            <input type="button" value="5" onclick="disp('5')">
        </td>
        <td>
            <input type="button" value="6" onclick="disp('6')">
        </td>
    </tr>
    <tr>
        <td>
            <input type="button" value="*" onclick="disp('*')">
        </td>
        <td>
            <input type="button" value="7" onclick="disp('7')">
        </td>
        <td>
            <input type="button" value="8"onclick="disp('8')">
        </td>
        <td>
            <input type="button" value="9" onclick="disp('9')">
        </td>
    </tr>
    <tr>
        <td>
            <input type="button" value="/" onclick="disp('/')">
        </td>
        <td>
            <input type="button" value="." onclick="disp('.')">
        </td>
        <td>
            <input type="button" value="0" onclick="disp('0')">
        </td>
        <td>
            <input type="button" value="=" onclick="solve()"  >
        </td>
    </tr>
 </table>

</body>
</html>
