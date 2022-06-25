<html>
 
<head>
    <title>
      Window moveBy() Method in HTML
    </title>
    <style>
        h1 {
            color: green;
        }
         
        h2 {
            font-family: Impact;
        }
         
        body {
            text-align: center;
        }
    </style>
</head>
 
<body>
 
    <h1>GeeksforGeeks</h1>
    <h2>Window moveBy() Method</h2>
 
    <p>
      For opening the Test window,
      double click the "Open Window" button:
    </p>
 
    <button ondblclick="Opwind()">
      Open Window
    </button>
    <br>
 
    <p>
      For moving the Test window,
      double click the "Move Window" button:
    </p>
 
    <button ondblclick="Movewind()">
      Move Window
    </button>
 
    <script>
        function Opwind() {
            TestWindow = window.open("", "TestWindow",
                "width=400, height=400");
            TestWindow.document.write("This is a Test Window.");
        }
 
        function Movewind() {
            TestWindow.moveBy(200, 200);
            TestWindow.focus();
        }
    </script>
 
</body>
 
</html>