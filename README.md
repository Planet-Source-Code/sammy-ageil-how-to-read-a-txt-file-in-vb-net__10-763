<div align="center">

## How to read a \.txt file in vb\.net


</div>

### Description

Just to show how to read a txt or .dat file in vb.net
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Sammy Ageil](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/sammy-ageil.md)
**Level**          |Beginner
**User Rating**    |4.7 (14 globes from 3 users)
**Compatibility**  |VB\.NET
**Category**       |[Files](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/files__10-2.md)
**World**          |[\.Net \(C\#, VB\.net\)](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/net-c-vb-net.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/sammy-ageil-how-to-read-a-txt-file-in-vb-net__10-763/archive/master.zip)





### Source Code

<table border="0" cellpadding="0" cellspacing="0" style="border-collapse: collapse" bordercolor="#111111" width="100%" id="AutoNumber1">
 <tr>
  <td width="50%">Private Sub btnReadTextFile_Click(ByVal sender _ As
  System.Object, ByVal e As System.EventArgs) _ Handles btnReadTextFile.Click</td>
  <td width="50%"><font color="#008000">'first lets create a form, add a
  command button on it and create a txt file called my textfile.txt and save
  it in C:\<br>
  paste this code into the click event of the command button<br>
&nbsp;</font></td>
 </tr>
 <tr>
  <td width="50%">Dim Strmyfile As String = FreeFile()<br>
  Dim strLine As String</td>
  <td width="50%"><font color="#008000">' first variable to hold our freefile
  you can<br>
  'replace it with a number if you wish<br>
&nbsp;</font></td>
 </tr>
 <tr>
  <td width="50%">FileOpen(Strmyfile, &quot;C:\FRONTPG.LOG&quot;, _ OpenMode.Input,
  OpenAccess.Read, _<br>
  OpenShare.Shared, -1)<br>
&nbsp;</td>
  <td width="50%"><font color="#008000">'once the file is opened <br>
  'loop through every line and copy them to our<br>
  'variable<br>
&nbsp;</font></td>
 </tr>
 <tr>
  <td width="50%">Do While Not EOF(Strmyfile)<br>
  strLine = LineInput(Strmyfile)<br>
  MsgBox(strLine)</td>
  <td width="50%"><font color="#008000">'copy the results to <br>
  'messagebox to show it<br>
&nbsp;</font></td>
 </tr>
 <tr>
  <td width="50%">&nbsp;Loop<br>
  End Sub</td>
  <td width="50%"><font color="#008000">Hit F5 to run the app</font></td>
 </tr>
<table>

