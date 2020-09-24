<div align="center">

## Disable program after 100 times used


</div>

### Description

This code will disable your program after a certain number of runs of the program. more info: worm@thepentagon.com
 
### More Info
 
Put in Form_Load statement. And this code is for 32-bit programming Only!

Don't put this code in while your testing and programming your program because it will then disable you from running your program. more info: worm@thepentagon.com


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Worm](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/worm.md)
**Level**          |Unknown
**User Rating**    |4.2 (165 globes from 39 users)
**Compatibility**  |VB 4\.0 \(32\-bit\), VB 5\.0, VB 6\.0
**Category**       |[Miscellaneous](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/miscellaneous__1-1.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/worm-disable-program-after-100-times-used__1-1518/archive/master.zip)





### Source Code

```
'put in form_load
retvalue = GetSetting("A", "0", "Runcount")
Worm$ = Val(retvalue) + 1
SaveSetting "A", "0", "RunCount", Worm$
If Worm$ > 99 Then 'put one number lower then it says....you can only run the program 200 times.
MsgBox "This is the end of the trial run",16,"Sorry"
Unload me
End If
```

