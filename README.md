Easing Loader
============

Easing Loader is a jquery plugin that uses easing functions and balls to create an animated loading graphic. 

Balls are animated across the width of a target div using whatever easing function you specify. To see a sample and play with some features, take a look at this fiddle: http://jsfiddle.net/wjmoody03/uyWcK/

###On Nuget
https://nuget.org/packages/EasedLoading/

###Usage
```javascript
  //to start the animation
  $("#targetDiv").loading();
  
  //to stop the animation graphic
  $("#targetDiv").loading(false);
```
####With Options
```javascript
  var options = {
    easing: "easeInOutCirc" 
  };
  
  //to start the animation
  $("#targetDiv").loading(options);
  
  //to stop the animation graphic
  $("#targetDiv").loading(false);
```



###Dependencies
  1. **Jquery** &gt;=1.0
  2. **Jquery Easing** &gt;=1.2 

###Options

<table>
  <tr>
    <th>Option</th>
    <th>Type</th>
    <th>Description</th>
    <th>Default</th>
  </tr>
  <tr>
    <td>easing</td>
    <td>String</td>
    <td>The name of the easing function to use. See this page for visualizations of the options: http://easings.net/ </td>
    <td>easeInOutQuart</td>
  </tr>
  <tr>
    <td>easing</td>
    <td>String</td>
    <td>The name of the easing function to use. See this page for visualizations of the options: </td>
    <td>easeInOutQuart</td>
  </tr>
  <tr>
    <td>animationDuration</td>
    <td>Number</td>
    <td>Milliseconds it takes the balls to traverse the target div (or complete the animation)</td>
    <td>4000</td>
  </tr>
  <tr>
    <td>newBallsInterval</td>
    <td>Number</td>
    <td>New balls will begin the animation at this interval of milliseconds</td>
    <td>400</td>
  </tr>
  <tr>
    <td>text</td>
    <td>String</td>
    <td>Display this text above the animated balls. Text will fade out as the remaining balls finish their animation.</td>
    <td></td>
  </tr> 
  <tr>
    <td>textClass</td>
    <td>String</td>
    <td>CSS class to apply to the text. This will override all default appearances of the text.</td>
    <td></td>
  </tr> 
  <tr>
    <td>ballClass</td>
    <td>String</td>
    <td>CSS class to apply to the balls being animated. The balls are simply animated spans, by default with a border radius and a background color. This class must have <code>position:absolute;</code> to work correctly.</td>
    <td></td>
  </tr>   
  <tr>
    <td>groupSize</td>
    <td>Number</td>
    <td>Batches balls in groups, then waits before sending the next group. If 0, it just sends a continuous stream of balls.</td>
    <td>0</td>
  </tr>     
</table>
