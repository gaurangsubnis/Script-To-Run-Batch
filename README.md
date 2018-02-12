# Script-To-Run-Batch
This script runs all the test cases in one run.

Set qtapp = CreateObject("QuickTest.Application")
qtApp.Launch
qtApp.Visible = True

qtApp.open "C:\Users\a584964\Documents\Unified Functional Testing\Practise", True
set qtTest=qtApp.Test
qtTest.Run
WScript.sleep 10000
qtTest.close

qtApp.open "C:\Users\a584964\Documents\Unified Functional Testing\Practise2", True
set qtTest=qtApp.Test
qtTest.Run
WScript.sleep 10000
qtTest.close


qtApp.quit

set qtTest=nothing
set qtApp=nothing
