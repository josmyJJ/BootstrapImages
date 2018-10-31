# BootstrapImages
## Learning Objectives
* Using bootstrap image styles

## The Walkthrough

1. Create a Spring Boot Application
	* Name it BootsrapImages
	* Add the dependencies for the web and for thymeleaf
	* Hit next until you finish the wizard, and then wait until it's done.

2. Create a Controller
	* Right click on com.example.demo and click New -> Class
	* Name it HomeController.java
	* Edit it to look like this:
```java
import org.springframework.stereotype.Controller;
import org.springframework.web.bind.annotation.RequestMapping;

@Controller
public class HomeController {

    @RequestMapping("/")
    public String index(){
        return "index";
    }
}
```

3. Create a Template
  * Right click on templates and click New -> Html
	* Name it index.html
	* Edit it to look like this:
```html
<!DOCTYPE html>
<html lang="en" xmlns:th="www.thymeleaf.org">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width,initial-scale=1">
    <title>Bootstrap 101 template</title>
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css" integrity="sha384-MCw98/SFnGE8fJT3GXwEOngsV7Zt27NXFoaoApmYm81iuXoPkFOJwJ8ERdknLPMO" crossorigin="anonymous">
</head>
<body>
<div class="container">
    <br>
    <h1>Images</h1>
    <h2>Responsive Image</h2>
    <img src="img/image.jpeg" class="img-fluid" alt="Responsive image">
    <h2>Image thumbnails</h2>
    <img src="img/image.jpeg" class="img-thumbnail" alt="Responsive image">
    <h2>Rounded</h2>
    <img src="img/image.jpeg" class="rounded" alt="Responsive image">
</div>
</body>
<script src="https://code.jquery.com/jquery-3.3.1.slim.min.js" integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo" crossorigin="anonymous"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.3/umd/popper.min.js" integrity="sha384-ZMP7rVo3mIykV+2+9J3UJ46jBk0WLaUAdn689aCwoqbBJiSnjAK/l8WvCWPIPm49" crossorigin="anonymous"></script>
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/js/bootstrap.min.js" integrity="sha384-ChfqqxuZUCnJSK3+MXmPNIyE6ZbWh2IMqE241rYiqJxyMiZ6OW/JmZQ5stwEULTy" crossorigin="anonymous"></script>
</html>
```

4. Run your application and open a browser, if you type in the URL http://localhost:8080

## What is Going On

### The Controller
Here, the default route maps to index.html.

### The View

#### Responsive images
img-fluid class is used to make the images responsive, so that it automatically adjust to fit the size of the parent element.

#### Image thumbnails
img-thumbnail gives the image a rounded 1px border around the image.

#### Rounded
Rounded class provide image rounded corners.
rounded-circle makes an oval shaped image.  

#### Image alining
By default images are aligned inline. Using the class float-left image can be aligned to the
left and float-right will align image to the right.

