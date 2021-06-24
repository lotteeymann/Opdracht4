# Opdracht4
Animation

![grass](https://user-images.githubusercontent.com/86419683/123307240-8ca28e80-d522-11eb-9c1b-dfbf0718968d.jpg)
![wood](https://user-images.githubusercontent.com/86419683/123307794-308c3a00-d523-11eb-95db-1fd5259077aa.jpg)
![wood2](https://user-images.githubusercontent.com/86419683/123307805-341fc100-d523-11eb-8fb4-efcb2c66b3af.jpg)


<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>Hello, WebVR! • A-Frame</title>
    <meta name="viewport" content="width=device-width">
    <script src="main.js"></script>
  </head>
  <body>
    <a-scene background="color: #333333">
      <a-assets>
          <img id="wood" src="wood.jpg" />
          <img id="wood2" src="wood2.jpg" />
          <img id="grass" src="grass.jpg" />
      </a-assets>
      <a-box id="myBox" 
        position="-1 2 -3" 
        rotation="0 45 0" 
        width="3" 
        height="1" 
        depth="1" 
        material="src: #wood"
        shadow 
        animation="property: rotation; 
                   to: 90 360 180; 
                   dur: 4000; 
                   easing: linear; 
                   loop: true" >
      </a-box>
      <a-box id="myOtherBox" 
        position="3 1 -3" 
        rotation="0 45 0" 
        width="3" 
        height="1" 
        depth="1" 
        material="src: #wood2"
        shadow>  
      </a-box>
      <a-plane id="ground"
        position="0 0 -4" 
        rotation="-90 0 0" 
        width="100" 
        height="100" 
        color="#7BC8A4" 
        material="src: #grass; repeat: 10 10"
        shadow>
      </a-plane> 
    </a-scene>
  </body>
</html>
