# BlindsComCodeChallenge

Blinds.com Coding Challenge for Candidate Charles Tatum II

This is the Blinds.com Coding Challenge issued by GCC. 

This challenge requires applicants to implement the Electronic Color Code for resistors as either an ASP.NET MVC web page, or
as a ReactJS page. This applicant chose Microsoft's ASP.NET MVC platform.

Details on the Electronic Color Code can be found on Wikipedia at this URL:
https://en.wikipedia.org/wiki/Electronic_color_code

Remember: this is implementing the color code for RESISTORS, not for capacitors or other components.


Prerequisites
=============

In order to run this project, you must have the following:

A Windows-based workstation running Visual Studio 2017. Community edition will suffice, but this project should run without
issues on the Professional, Ultimate or Enterprise versions as well.
   

Setup
=====

1.  Download all project files as a set into the folder of choice.

2.  Start Visual Studio 2017.

3.  From the menu bar, choose File >> Open >> Project/Solution...

4.  Navigate to the folder where you placed the project files. You will have reached the correct folder when you see a file
    called "OhmValueCalc.sln".
    
5.  Double-click on the OhmValueCalc.sln file (or, alternatively, click once on the OhmValueCalc.sln file and then click the 
    "Open" button).
    

Compile
=======

1.  To compile and run/start the project, press F5, or click the browser selector near the top of the screen. The default 
    browser will be "Microsoft Edge" (if running on Windows 10), but you may choose another browser if you wish.
    
2.  After a few moments, Visual Studio will start IIS Express (a miniature web server) as well as the browser you chose.
    The web page will be hosted at "localhost" using a randomly chosen 5-digit port number.
    
    
Run
===

1.  To run the calculator, simply click on any of the color swatch names on the lines marked "Band 1", "Band 2", "Band 3", and
    "Band 4".  Your selections will be shown to the immediate right of these four labels. 
    
2.  When you have selected all four band colors, click the blue "Calculate" button.  Immediately beneath the button, you are 
    shown the resistance in Ohms, followed by the tolerance expressed as a percentage.
    
    
Unit Testing
============

1.  To run the 35 unit tests included in the Visual Studio solution, first be sure that the web page is no longer running by
    closing the web browser and clicking the Stop button (a red block icon) on the toolbar at the top of the screen.
    
2.  Start the unit tests by choosing the following from the menu bar: Tests >> Run >> All Tests.

3.  The Test Explorer window should appear, showing the results of all tests (all green check marks for success).


Notes
=====

1.  The original requirements for this challenge specified the following method to be created:

          int CalculateOhmValue(string bandAColor, string bandBColor, string bandCColor, string bandDColor);

    Because Ohm values can be fractions, this method was changed to return a double-precision value instead. Calculations
    throughout this project are conducted in either floating-point or double-precision numbers.
    
2.  The design of the UI does not permit the user to make a mistake of any kind.  The text boxes are set to read-only, and
    are associatd with the ResistorModel used by the page.  Each of the four band color values can only be set by clicking
    on the color swatches.
    
3.  Along with the above point, if a color does not apply to a particular band, it is not shown in the choices the user 
    can make.
    
