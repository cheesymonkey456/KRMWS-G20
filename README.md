# KRMWS-G20
* index.html:
```
  <!DOCTYPE html>
<html lang="en">
<head>
    <link rel="stylesheet" href="index.css">
</head>
<body>
    <div class="loader">Loading...</div>
<!-- content div from here -->
<!-- make div with id="content" -->
<div id="content" style="display: none;">
<div class="text-container">

            <h1>Technocrat 1.0 presentation</h1>
            <h1>Topic: Impact of education of G20 in India</h1>
            <h2 class="krm">K.R. Mangalam World School, G.K. II</h2>
            <p>by Sabeeir Sharrma and Manikya Porwal (class IX)</p>
            <a class="ht1" href="selection.html">continue</a>
        </div>
    </div>

    <script src="js/index.js"></script>
</body>
</html>
```
* index.css
```
   * {
    padding: 0px;
    margin: 0px;
    box-sizing: border-box;
    justify-content: center;
    align-items: center;
}

html {
    height: 100%;
    scroll-behavior: smooth;
}
body {
    background: #363636; /* Set the background color to black */
    margin: 0; /* Remove default margin */
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;

  }
  .text-container {
  overflow: hidden;
}
  .ea {
    opacity: 0;
      transform: translateX(-100%);
  animation: slide-in 1s forwards;
  }
  .loader {
    width: 250px;
    height: 50px;
    
    line-height: 50px;
    text-align: center;
    font-family: helvetica, arial, sans-serif;
    text-transform: uppercase;
    font-weight: 900;
    color: #e0e0e0;
    letter-spacing: 0.2em;
    
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);  
  }
  .loader::before,
  .loader::after {
    content: "";
    display: block;
    width: 15px;
    height: 15px;
    background: #e0e0e0;
    position: absolute;
    animation: load 0.9s infinite alternate ease-in-out;
  }
  .loader::before {
    top: 0;
  }
  .loader::after {
    bottom: 0;
  }
  
  @font-face {
    font-family: "Ubuntu";
    src: url(https://fonts.googleapis.com/css?family=Ubuntu:300,300italic,reuglar,italic,500,500italic,700,700italic);
  }
  
  @keyframes load {
    0% {
      left: 0;
      height: 30px;
      width: 15px;
    }
    50% {
      height: 8px;
      width: 40px;
    }
    100% {
      left: 235px;
      height: 30px;
      width: 15px;
    }
  }
  h1 {
    font-size: 40px;
    color: #e0e0e0;
    font-family: helvetica, arial, sans-serif;
    text-transform: uppercase;
    font-weight: 900;
    justify-content: center;
    align-items: left;
    display: inline-block;
    position: relative;
  }
  h1:after {
    content: '';
    position: absolute;
    width: 100%;
    transform: scaleX(0);
    height: 7px;
    bottom: 0;
    left: 0;
    background-color: #0088a9;
    transform-origin: bottom right;
    transition: transform 0.3s ease-out;
  }
  h1:hover:after {
    transform: scaleX(1);
    transform-origin: bottom left;
  }
  p {
    padding-top: 20px;
    font-size: 20px;
    color: #e0e0e0;
    font-family: Arial, Helvetica, sans-serif;
    font-weight: 900;
    justify-content: center;
    align-items: center;
    transition: all 0.3s ease;
  }
  p:hover {
    margin-left: 15px;
    color: #0088a9;
  }
  .krm {
    padding-top: 20px;
    font-size: 20px;
    color: #e0e0e0;
    font-family: Arial, Helvetica, sans-serif;
    font-weight: 900;
    justify-content: center;
    align-items: center;
    transition: all 0.3s ease;
  }
  .krm:hover {
    margin-left: 15px;
    color: #ff1900;
  }
  .ht1 {
            display: inline-block;
            padding: 10px 20px;
            font-size: 24px;
            background-color: #007BFF;
            color: #FFF;
            text-decoration: none;
            border-radius: 5px;
            margin-top: 20px;
            transition: all 0.3s ease;

        }
  .ht1:hover {
    background-color: #3e659c;
    margin-left: 50px;
  }
.image-container {
  display: flex;
  align-items: center;
  padding: 20px;
}

img {
  max-width: 100%;
  height: auto;
  margin-right: 20px;
}
 .ht2 {
            display: inline-block;
            padding: 10px 20px;
            font-size: 24px;
            background-color: #007BFF;
            color: #FFF;
            text-decoration: none;
            border-radius: 5px;
            margin-top: 20px;
            transition: all 0.3s ease;

        }
  .ht2:hover {
    background-color: #3e659c;
    margin-top: 50px;
  }
  ```
* selection screen:
```
<!DOCTYPE html>
<html lang="en">
<head>
    <link rel="stylesheet" href="index.css">
</head>
<body>
<!-- content div from here -->
<!-- make div with id="content" -->
<div name="select">
    <div class="text-container">        
            <h1>Technocrat 1.0 presentation</h1>
            <h1>Topic: Impact of education of G20 in India</h1>
            <h2 class="krm">K.R. Mangalam World School, G.K. II</h2>
            <p>by Sabeeir Sharrma and Manikya Porwal (class IX)</p>
            <a class="ht1" href="https://www.onworks.net/owncloud/index.php/s/Yhv66s6jWWYDXp2/download">Download PPT for Better Understanding</a>
            <a class="ht1" href="slide1.html">View Web Presentation &#8594;</a>
        </div>
    </div>

</body>
</html>
```
* css animations
```
.fade-in {
  opacity: 0; /* Initially hidden */
  transform: translateY(20px); /* Move down slightly */
  animation: fadeInAnimation 1.5s ease-in-out forwards; /* Apply animation */
}

@keyframes fadeInAnimation {
  from {
    opacity: 0;
    transform: translateY(20px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
  h1 {
    font-size: 40px;
    color: #e0e0e0;
    font-family: helvetica, arial, sans-serif;
    text-transform: uppercase;
    font-weight: 900;
    justify-content: center;
    align-items: left;
    display: inline-block;
    position: relative;
  }
  h1:after {
    content: '';
    position: absolute;
    width: 100%;
    transform: scaleX(0);
    height: 7px;
    bottom: 0;
    left: 0;
    background-color: #0088a9;
    transform-origin: bottom right;
    transition: transform 0.3s ease-out;
  }
  h1:hover:after {
    transform: scaleX(1);
    transform-origin: bottom left;
  }
  p {
    padding-top: 20px;
    font-size: 20px;
    color: #e0e0e0;
    font-family: Arial, Helvetica, sans-serif;
    font-weight: 900;
    justify-content: center;
    align-items: center;
    transition: all 0.3s ease;
    padding-bottom: 6px;
  }
  p:hover {
    margin-left: 15px;
    color: #0088a9;
  }
  .ht1 {
            display: inline-block;
            padding: 10px 20px;
            font-size: 24px;
            background-color: #007BFF;
            color: #FFF;
            text-decoration: none;
            border-radius: 5px;
            margin-top: 20px;
            transition: all 0.3s ease;
            align-items: center;
            justify-content: center;
        }
  .ht1:hover {
    background-color: #3e659c;
  }
.ht2 {
            display: inline-block;
            padding: 10px 20px;
            font-size: 24px;
            background-color: #007BFF;
            color: #FFF;
            text-decoration: none;
            border-radius: 5px;
            margin-top: 20px;
            transition: all 0.3s ease;
            align-items: center;
            justify-content: center;
        }
  .ht2:hover {
    background-color: #3e659c;
  }
.point {
    font-family: Arial, Helvetica, sans-serif;
    font-weight: 900;
    justify-content: center;
    align-items: center;
    transition: all 0.3s ease;
    color: #0088a9;
}
.pt {
    font-family: Arial, Helvetica, sans-serif;
    font-weight: 900;
    justify-content: center;
    align-items: center;
    transition: all 0.3s ease;
    color: #e0e0e0;
}
.ps {
    font-size: 20px;
    color: #e0e0e0;
    font-family: helvetica, arial, sans-serif;
    text-transform: uppercase;
    font-weight: 900;
    justify-content: center;
    align-items: left;
    display: inline-block;
    position: relative;
}
.ps:hover {
    margin-left: 15px;
    color: #0088a9;
}
```
