# Helper
## A helper class with many tools from php

## BEFORE START
You have to define a ROOT constant which will be used for links to find the correct route,
In this example we would be using '/app' as our ROOT
define('ROOT','/app')
## Methods

**link_to:**
  - Static method
  Writes a link to a defined controller/action in a project
  USAGE: Helper::link_to(String $controller,String $action,String $text,Array $options);
  
  Parameters
    $controller = The controller to redirect
    $action = The action to redirect
    $options = An associative array where all html attributes should be;
    $text=The text that will be shown on the link
    
 Example:
  *Let's make a link to articles/new*
  
 `<?= Helper::link_to('articles','new','Hello World!',['style'=>'color:red','id'=>'mylink','class'=>'link']) ?>`
 
  The resulting HTML will be:
  
 `<a href="/app/articles/new" style='color:red' id='mylink' class='link'>Hello world!</a>`
  
  
