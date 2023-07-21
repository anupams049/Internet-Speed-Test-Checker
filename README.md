# Internet-Speed-Test-Checker
Easily Check Internet Speed by using this tool
<!DOCTYPE html>
<html>
<head>
  <title>Fast.com Web View</title>
  <style>
    html, body {
      margin: 0;
      padding: 0;
      height: 100%;
    }
    #webview {
      width: 100%;
      height: 100%;
      border: none;
    }
  </style>
</head>
<body>
  <iframe id="webview"></iframe>

  <script>
    window.onload = function() {
      var webview = document.getElementById("webview");

      function resizeWebview() {
        webview.style.height = window.innerHeight + "px";
      }

      // Resize the web view when the window is resized
      window.addEventListener("resize", resizeWebview);

      // Load the Fast.com website into the web view
      webview.src = "https://fast.com";

      // Initially resize the web view
      resizeWebview();
    };
  </script>
</body>
</html>
