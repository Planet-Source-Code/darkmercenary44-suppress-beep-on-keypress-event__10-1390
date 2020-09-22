<div align="center">

## Suppress Beep on KeyPress Event


</div>

### Description

This article will quickly and to the point show you how to supress the beep when the user presses the enter key in a single line text box.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[DarkMercenary44](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/darkmercenary44.md)
**Level**          |Beginner
**User Rating**    |4.8 (19 globes from 4 users)
**Compatibility**  |VB\.NET
**Category**       |[Controls/ Forms/ Dialogs/ Menus](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/controls-forms-dialogs-menus__10-3.md)
**World**          |[\.Net \(C\#, VB\.net\)](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/net-c-vb-net.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/darkmercenary44-suppress-beep-on-keypress-event__10-1390/archive/master.zip)





### Source Code

<p>All you have to do is set the e.Handled to True and no beeps.<br>
Example:</p>
<font COLOR="#0000FF">
<p>Private Sub</font><font COLOR="#ffffff"> </font><font COLOR="#ff00ff">
txt_Input_KeyPress</font><font COLOR="#ffffff">(</font><font COLOR="#0000FF">ByVal</font><font COLOR="#ffffff">
</font><font COLOR="#ff00ff">sender</font><font COLOR="#ffffff"> </font>
<font COLOR="#0000FF">As Object, ByVal</font><font COLOR="#ffffff"> </font>
<font COLOR="#ff00ff">e</font><font COLOR="#ffffff"> </font>
<font COLOR="#0000FF">As</font><font COLOR="#ffffff"> </font>
<font COLOR="#ff00ff">System</font>.<font COLOR="#ff00ff">Windows</font>.<font COLOR="#ff00ff">Forms</font>.<font COLOR="#ff00ff">KeyPressEventArgs</font><font COLOR="#ffffff">)
</font><font COLOR="#0000FF">Handles</font><font COLOR="#ffffff"> </font>
<font COLOR="#ff00ff">txt_Input</font>.<font COLOR="#ff00ff">KeyPress</p>
</font><font SIZE="1" COLOR="#ffffff">
<blockquote>
 <p></font><font COLOR="#0000FF">If</font><font COLOR="#ffffff"> </font>
 <font COLOR="#ff00ff">e</font>.<font COLOR="#ff00ff">KeyChar</font><font COLOR="#ffffff">
 </font><font color="#FF0000">=</font><font COLOR="#ffffff"> </font>
 <font COLOR="#ff00ff">Chr</font>(<font COLOR="#FF0000">13</font>)<font COLOR="#ffffff">
 </font><font COLOR="#0000FF">Then</p>
 </font><font SIZE="1" COLOR="#ffffff">
 <blockquote>
  <p></font><font COLOR="#ff00ff">Console</font>.<font COLOR="#ff00ff">WriteLine</font>(<font COLOR="#808080">&quot;ENTER</font><font COLOR="#808080">
  PRESSED&quot;</font>)</p>
  <p><font COLOR="#ff00ff">e</font>.<font COLOR="#ff00ff">Handled</font><font COLOR="#ffffff">
  </font><font color="#FF0000">=</font><font COLOR="#ffffff"> </font>
  <font COLOR="#0000FF">True</p>
 </blockquote>
 </font><font SIZE="1" COLOR="#ffffff">
 <p></font><font COLOR="#0000FF">End If</p>
</blockquote>
</font><font SIZE="1" COLOR="#ffffff">
<p></font><font COLOR="#0000FF">End Sub</p>
</font>

