# Fixing "font not embedded" issue to pass the IEEE PDF eXpress check

I spent two hours making my pdf file to pass the IEEE PDF eXpress check.

After I latex and submit the pdf file, I got the following errors.

Errors & Warnings
Severity Description
? 8 Error Font TimesNewRomanPSMT is not embedded (817x)
? 8 Error Font TimesNewRomanPS-ItalicMT is not embedded (204x)
? 8 Error Font TimesNewRomanPS-BoldItalicMT is not embedded (6x)
? 8 Error Font TimesNewRomanPS-BoldMT is not embedded (13x)
? 8 Error Font Arial-ItalicMT is not embedded
? 8 Error Font ArialMT is not embedded (12x) 


You may also get other fonts embedding problem.


In Windows, the solution can be very simple.


    1. open your pdf file, 
    2. select file -> print
    3. set your printer to be Adobe printer (assuming you already installed it)
    4. click on properties
    5. click the tab "Adobe PDF Settings"
    6. uncheck "Rely on system fonts only; do not use document fonts"
    7. click on the Edit... after Default Settings
    8. click on Fonts, add those missing fonts to "Always Embed" (It is recommended to save the properties as a new setting.)
    9. print the pdf file with the new settings, and your new pdf file should be good to go.
