# ActionSlideJS
Ready? Steady? Action!

![alt tag](http://lironaichel.com/jsworks/actionslide/css3.jpg)

Simple animation library for action movie credits (aka "action slide") in JavaScript, supporting all major browsers:
 * IE9+
 * Firefox
 * Safari
 * Chrome
 * Opera
 
**Prerequisite: JQuery**

Copyright (c) 2013 - 2013 Liron Aichel <br/>

Project homepage: http://lironaichel.com/jsworks/actionslide/ <br/>
Github homepage: http://liri.github.io/ActionSlideJS. <br/>

CSS3 Demo: http://lironaichel.com/jsworks/actionslide/samples/css3Background.html <br/>
Documentation: http://lironaichel.com/jsworks/actionslide/docs/index.html <br/>

Licensed under MIT-style license:
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 <div class="span8">
                    	<section id="started"> 
                            <div class="page-header">
                                <h1>Getting Started</h1>
                            </div>
                            <p>
                            ActionSlideJS is a tiny animation library for creating a "action movie opening" like animation (also works as jQuery plugin).
                            <br/>
                            To start use ActionSlideJS, include jQuery library:
                            </p>
<pre ><code>  <span style="color:#687687">&lt;</span>script src<span style="color:#687687">=</span><span style="color:#036a07">"js/jquery.min.js"</span><span style="color:#687687">></span><span style="color:#687687">&lt;</span>/script<span style="color:#687687">></span>
</code></pre>

                            Include ActionSlideJS library:

<pre ><code>  <span style="color:#687687">&lt;</span>script src<span style="color:#687687">=</span><span style="color:#036a07">"js/actionslide.min.js"</span><span style="color:#687687">></span><span style="color:#687687">&lt;</span>/script<span style="color:#687687">></span>
</code></pre>
							<p>
                            Include ActionSlideJS styling (CSS):
                            </p>
<pre ><code>  <span style="color:#687687">&lt;</span>link rel<span style="color:#687687">=</span><span style="color:#036a07">"stylesheet"</span> type<span style="color:#687687">=</span><span style="color:#036a07">"text/css"</span> href<span style="color:#687687">=</span><span style="color:#036a07">"css/actionslide.css"</span> /<span style="color:#687687">></span>
</code></pre>
							<h4>You're good to go!</h4>
						</section>
                        <section id="basic"> 
                            <div class="page-header">
                                <h1>Basic example</h1>
                            </div>
                                           
                            <h2>Zero lines of code!</h2>
                            <p>
                            ActionSlideJS automatically detect your DOM element. Just place "data-role='actionSlide'" on your list element (ul):
                            </p>
<pre class="prettyprint linenums">
  <span style="color:#1c02ff">&lt;<span style="font-weight:700">ul</span> <span style="font-style:italic">data-role</span>=<span style="color:#036a07">"actionSlide"</span>></span>
        <span style="color:#1c02ff">&lt;<span style="font-weight:700">li</span> <span style="font-style:italic">data-title</span>=<span style="color:#036a07">"Slide I"</span> <span style="font-style:italic">data-duration</span>=<span style="color:#036a07">"3000"</span>></span>
            <span style="color:#1c02ff">&lt;<span style="font-weight:700">span</span>></span>Slide I Content<span style="color:#1c02ff">&lt;/<span style="font-weight:700">span</span>></span>
        <span style="color:#1c02ff">&lt;/<span style="font-weight:700">li</span>></span>
        <span style="color:#1c02ff">&lt;<span style="font-weight:700">li</span> <span style="font-style:italic">data-title</span>=<span style="color:#036a07">"Slide II"</span> <span style="font-style:italic">data-duration</span>=<span style="color:#036a07">"2000"</span>></span>
            <span style="color:#1c02ff">&lt;<span style="font-weight:700">span</span>></span>Slide II Content<span style="color:#1c02ff">&lt;/<span style="font-weight:700">span</span>></span>
        <span style="color:#1c02ff">&lt;/<span style="font-weight:700">li</span>></span>
<span style="color:#1c02ff">&lt;/<span style="font-weight:700">ul</span>
</span></pre>
                        </section>
                        <section id="options">
                            <div class="page-header">
                                <h1>Helpful options</h1>
                            </div>
                            <h2>Stage Animation</h2>
                            <p>There is an option to animate background lines, you can disable it using:</p>
                            <h3>data-animate-background</h3>
<pre class="prettyprint linenums">
<span style="color:#1c02ff">&lt;<span style="font-weight:700">ul</span> <span style="font-style:italic">data-role</span>=<span style="color:#036a07">"actionSlide"</span> <span style="font-style:italic">data-animate-background</span>=<span style="color:#036a07">"false"</span>></span></pre>
                            <p>It's pretty cool and enhanch the "action" style.</p>

                            <h2>Slide Animation</h2>
                            <p>Each slide has default properties during the slideshow:</p>
                            <ul>
                              <li>title = (empty)</li>
                              <li>duration = 2000 (2 seconds)</li>
                              <li>animation = slide</li>
                              <li>direction = left-to-right</li>
                              <li>textAlign = left</li>
                              <li>easing = linear</li>
                              </li>
                            </ul>
                            <p>You can change any of the default values using "data-" on each slide element (li).</p>

                         	<h3>data-title</h3>
                            <p>
                            Appears as the slide title, different just in style from the slide content.
                            </p>
                            <pre class="prettyprint linenums">
<span style="color:#1c02ff">&lt;<span style="font-weight:700">li</span> <span style="font-style:italic">data-title</span>=<span style="color:#036a07">"Slide I"</span>></span></pre>
	
                            <h3>data-duration</h3>
                            <p>
                            The duration of the slide animation.
                            </p>
                            <pre class="prettyprint linenums">
<span style="color:#1c02ff">&lt;<span style="font-weight:700">li</span> <span style="font-style:italic">data-duration</span>=<span style="color:#036a07">"5000"</span>></span></pre>

                            <h3>data-animation</h3>
                            <p>
                            The animaiton type for this slide, possible values are currently 'fade' or 'slide'.
                            </p>
                            <pre class="prettyprint linenums">
<span style="color:#1c02ff">&lt;<span style="font-weight:700">li</span> <span style="font-style:italic">data-animation</span>=<span style="color:#036a07">"slide/fade"</span>></span></pre>

                            <h3>data-direction</h3>
                            <p>
                            Only relevant for 'slide' animation. Controls the direction of the animation, possible values are 'rtl' or 'ltr'.
                            </p>
                            <pre class="prettyprint linenums">
<span style="color:#1c02ff">&lt;<span style="font-weight:700">li</span> <span style="font-style:italic">data-direction</span>=<span style="color:#036a07">"rtl/ltr"</span>></span></pre>

                            <h3>data-textAlign</h3>
                            <p>
                            The slide content text alignment.
                            </p>
                            <pre class="prettyprint linenums">
<span style="color:#1c02ff">&lt;<span style="font-weight:700">li</span> <span style="font-style:italic">data-textAlign</span>=<span style="color:#036a07">"center"</span>></span></pre>

                            <h3>data-easing</h3>
                            <p>
                            The easing function of the slide animation.
                            </p>
                            <pre class="prettyprint linenums">
<span style="color:#1c02ff">&lt;<span style="font-weight:700">li</span> <span style="font-style:italic">data-easing</span>=<span style="color:#036a07">"linear"</span>></span></pre>                      
                            <p class="alert alert-info">
                              Using easing functions other than 'linear' requires jQuery UI library.
                            </p>
                        </section>

                      <section id="css">
                            <div class="page-header">
                                <h1>CSS Customization</h1>
                            </div>                           
                            <p>ActionSlideJS works on top of your container element, you can style the container as you wish.
                            <br />
                            In order to match ActionSlideJS styling to your container, use the following classes:</p>

                            <h4>actionslide-container</h4>
                            <p>Container for each animated slide.</p>
                            <pre class="prettyprint linenums">
<span style="font-style:italic">.actionslide-container</span> <span style="font-weight:700">a</span> {
    <span style="color:#6d79de;font-weight:700">color</span>: <span style="color:#06960e;font-weight:700">white</span>;
    <span style="color:#6d79de;font-weight:700">text-decoration</span>: <span style="color:#06960e;font-weight:700">underline</span>;
}

<span style="font-style:italic">.actionslide-container</span> <span style="font-weight:700">a</span><span style="font-style:italic">:hover</span> {
    <span style="color:#6d79de;font-weight:700">text-decoration</span>: <span style="color:#06960e;font-weight:700">none</span>;
}
</pre>
                            <h4>actionslide-title</h4>
                            <p>Slide title style</p>
                            <pre class="prettyprint linenums">
<span style="font-style:italic">.actionslide-title</span> {
    <span style="color:#6d79de;font-weight:700">font-size</span>: <span style="color:#0000cd">34<span style="color:#00f;font-weight:700">px</span></span>; 
    <span style="color:#6d79de;font-weight:700">font-style</span>: <span style="color:#06960e;font-weight:700">italic</span>; 
    <span style="color:#6d79de;font-weight:700">font-weight</span>: <span style="color:#06960e;font-weight:700">bold</span>; 
    <span style="color:#6d79de;font-weight:700">color</span>: <span style="color:#06960e;font-weight:700">black</span>; 
    <span style="color:#6d79de;font-weight:700">margin-bottom</span>: <span style="color:#0000cd">10<span style="color:#00f;font-weight:700">px</span></span>;
    <span style="color:#6d79de;font-weight:700">text-shadow</span>: <span style="color:#0000cd">-1<span style="color:#00f;font-weight:700">px</span></span> <span style="color:#0000cd">-1<span style="color:#00f;font-weight:700">px</span></span> <span style="color:#c5060b;font-weight:700">#bbb</span>,<span style="color:#0000cd">1<span style="color:#00f;font-weight:700">px</span></span> <span style="color:#0000cd">1<span style="color:#00f;font-weight:700">px</span></span> <span style="color:#c5060b;font-weight:700">#bbb</span>;
    <span style="color:#6d79de;font-weight:700">color</span>:<span style="color:#c5060b;font-weight:700">#eee</span>;
    <span style="color:#6d79de;font-weight:700">letter-spacing</span>: <span style="color:#0000cd">2<span style="color:#00f;font-weight:700">px</span></span>;
}</pre>
                            <h4>actionslide-content</h4>
                            <p>Slide content style</p>
                            <pre class="prettyprint linenums">
<span style="font-style:italic">.actionslide-content</span> {
    <span style="color:#6d79de;font-weight:700">font-size</span>: <span style="color:#0000cd">18<span style="color:#00f;font-weight:700">px</span></span>; 
    <span style="color:#6d79de;font-weight:700">text-shadow</span>: <span style="color:#0000cd">-1<span style="color:#00f;font-weight:700">px</span></span> <span style="color:#0000cd">-1<span style="color:#00f;font-weight:700">px</span></span> <span style="color:#c5060b;font-weight:700">#bbb</span>,<span style="color:#0000cd">1<span style="color:#00f;font-weight:700">px</span></span> <span style="color:#0000cd">1<span style="color:#00f;font-weight:700">px</span></span> <span style="color:#c5060b;font-weight:700">#bbb</span>;
    <span style="color:#6d79de;font-weight:700">color</span>:<span style="color:#c5060b;font-weight:700">#eee</span>;
}</pre>
                            <h4>actionslide-bglines</h4>
                            <p>Background lines animation</p>
                            <pre class="prettyprint linenums">
<span style="font-style:italic">.actionslide-bglines</span> {
    <span style="color:#6d79de;font-weight:700">height</span>: <span style="color:#0000cd">2<span style="color:#00f;font-weight:700">px</span></span>; 
    <span style="color:#6d79de;font-weight:700">background-color</span>: <span style="color:#06960e;font-weight:700">white</span>; 
    <span style="color:#6d79de;font-weight:700">opacity</span>: <span style="color:#0000cd">0.1</span>
}
</pre>
                        </section>         
                    </div>

[![Analytics](https://ga-beacon.appspot.com/UA-5480161-11/ActionSlideJS/readme)](https://github.com/igrigorik/ga-beacon)
