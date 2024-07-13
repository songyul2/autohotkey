# autohotkey
https://stackoverflow.com/questions/41723490/how-to-build-ahk-scripts-automatically-on-startup 
Simply add a shortcut of your script in the Windows 'Startup' folder.

Three ways to get there:

1- In Windows Explorer, go to %APPDATA%\Microsoft\Windows\Start Menu\Programs\Startup (for current user startup list) or %ALLUSERSPROFILE%\Microsoft\Windows\Start Menu\Programs\Startup (for every user startup list)

or

2- Open Windows' Run application (Windows + r) write shell:startup (current user) or shell:common startup (every user) in the edit field and click on the 'ok' button.

<code>
#SuspendExempt
!s::Suspend  ; Alt+S
#SuspendExempt False
1::!
2::@
3::#
4::$
5::% 
6::^
7::&
8::*
9::(
0::)
$+1::send 1
$+2::send 2
$+3::send 3
$+4::send 4
$+5::send 5
$+6::send 6
$+7::send 7
$+8::send 8
$+9::send 9
$+0::send 0
</code>
