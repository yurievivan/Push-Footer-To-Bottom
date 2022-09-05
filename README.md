<h1>Three ways to push the footer to the bottom of the page.</h1>
<p>Consider 3 ways, where the first 2 ways are using flexbox and the last third is using grid. Below is a simple example of a small page. A page consists of a general container "page", "header", "content" and "footer."</p>
<h4>HTML and CSS Code</h4>
<div align="center"><img src="https://user-images.githubusercontent.com/11561851/188332635-be460613-7bfc-4fe5-936d-e26cc3d82e13.png"></div>
<h3>1. With Flexbox and Margin</h3>
<p>For the "page" class, add the following styles:</p> <pre>
   <code class="language-css">
.page {
    display: flex;
    flex-direction: column;
    min-height: 100vh;
    overflow: hidden;
}
   </code>
</pre>
<p>For the "footer" class, just add <b>margin-top: auto</b>. See below:</p> <pre>
   <code class="language-css">
.footer {
    margin-top: auto;
}
   </code>
</pre>
<h3>2. With Only Flexbox</h3>
<p>For the "page" class, we add everything the same as for the first way.</p> <pre>
   <code class="language-css">
.page {
    display: flex;
    flex-direction: column;
    min-height: 100vh;
    overflow: hidden;
}
   </code>
</pre>
<p>For the "content" class, just add <b>flex: 1 1 auto</b>. See below:</p> <pre>
   <code class="language-css">
.content {
    flex: 1 1 auto;
}
   </code>
</pre>
<p>The CSS <b>flex: 1 1 auto</b> property is shorthand. It is short for <b>flex-grow</b>, <b>flex-shrink</b> and <b>flex-base</b>. The same property can be represented as follows:</p> <pre>
   <code class="language-css">
.content {
    <b>flex-grow: 1;</b>
    <b>flex-shrink: 1;</b>
    <b>flex-basis: auto;</b>
}
   </code>
</pre>
<h3>3. With Grid</h3>
<p>For the "page" class, add the following styles:</p> <pre>
   <code class="language-css">
.page {
    display: grid;
    grid grid-template-areas: "header" "content" "footer";
    grid-template-rows: auto 1fr auto;
    min-height: 100vh;
    overflow: hidden;
}
   </code>
</pre>
