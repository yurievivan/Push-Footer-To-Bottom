<h1>Three ways to push the footer to the bottom of the page.</h1>
<p>Consider 3 ways, where the first 2 ways are using flexbox and the last third is using grid. Below is a simple example of a small page. A page consists of a general container "page", "header", "content" and "footer."</p>
<h4>HTML and CSS Code</h4>
<div align="center"><img src="https://user-images.githubusercontent.com/11561851/188332635-be460613-7bfc-4fe5-936d-e26cc3d82e13.png"></div>
<h4>1. With flexbox and margin</h4>
<p>For the "page" class, add the following styles:</p>
<pre>
   <code class="language-css">
.page {
    display: flex;
    flex-direction: column;
    min-height: 100vh;
    overflow: hidden;
}
   </code>
</pre>
<p>For the "footer" class, just add margin-top: auto. See below:</p>
<pre>
   <code class="language-css">
.footer {
    margin-top: auto;
}
   </code>
</pre>
