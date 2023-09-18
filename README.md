<h2>Basic usage</h2>

Include a link to the styles:

```html
<link rel="stylesheet" href="css/styles.css">
```


````html

<!DOCTYPE html>
<html lang="en">
   <head>

      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <meta http-equiv="X-UA-Compatible" content="ie=edge">
      <title>Document</title>
            <script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.7.2/highlight.min.js"></script>
      <script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.7.2/languages/javascript.min.js"></script>
      <script>
         hljs.highlightAll();
      </script>
      <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.8.0/styles/base16/humanoid-dark.min.css" integrity="sha512-VpzmzXvIXjYfKE4xjvTjF41gt15bbXf3u0CDWXDm105TA7yphqLSVqAc+gnpJswiS068uRYqiXCC4MvCycjQhg==" crossorigin="anonymous" referrerpolicy="no-referrer" />
      
   </head>
   <body>
      <!--      Start       -->
      <pre style="width: 90vw; margin: auto; position: relative; display: flex; flex-wrap: nowrap; margin-bottom: 20px; border: 2px solid gray; background: #f5f5f5; overflow-x: auto; border-radius: 10px; background: #000; max-height: 40vh;color: white;"><code style="background: black;" class="language-html">
      &lt;!--      Start       --&gt;
               
               
               

        &lt;div class="response"&gt;
           &lt;pre&gt;&lt;code style="background: black;" class="language-html"&gt;
 
   
            &lt;/code&gt;&lt;/pre&gt;
           &lt;button class="copy-button"&gt;Copy.    &lt;/button&gt;
        &lt;/div&gt;

      
      &lt;!--      End       --&gt;

 
   
 
   
            </code><button class="copy-button" style="position: absolute; top: 10px; right: 10px; height: 25px; padding: 4px 8px; border: none; border-radius: 4px; background-color: #007bff; color: #fff; cursor: pointer;" onclick="copyResponseText(this)">Copy</button>

      </pre>
      <!--      End       -->

       
      <script>
         function copyResponseText() {
           const responseTextElement = this.previousElementSibling;
           const textToCopy = responseTextElement.innerText;
         
          
           const tempTextArea = document.createElement('textarea');
           tempTextArea.value = textToCopy;
           document.body.appendChild(tempTextArea);
         
         
           tempTextArea.select();
           document.execCommand('copy');
         
           
           document.body.removeChild(tempTextArea);
         
         
           this.innerText = 'Copied!';
           setTimeout(() => {
             this.innerText = 'Copy';
           }, 2000);
         }
         
         
         const copyButtons = document.querySelectorAll('.copy-button');
         copyButtons.forEach((button) => {
           button.addEventListener('click', copyResponseText);
         });
      </script>
   </body>
</html> 
   
                

                
````


Add content block(s) with data attribute (value = number of lines to display).

```html
<div class="CCR">
  <div class="CCR_txt" data-cropCopyRestore="2">
    Content copy...
  </div>
</div>
```

Include a link to the script:

```html
<script src="js/cropCopyRestore.2.1.min.js"></script>
```

<br>
<h2>Features</h2>
