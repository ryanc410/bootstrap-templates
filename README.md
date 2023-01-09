# Custom Bootstrap Templates
Collection of bootstrap templates with custom styling

# FILES
Click on the links below for an explanation on how I use the files and how you can customize it for your project 
- <a href="https://github.com/ryanc410/bootstrap-templates/edit/main/README.md#navbar_login_signup_modalshtml">Bootstrap Navbar with Login and Signup Form Modals</a>

## `navbar_login_signup_modals.html`

I broke this file up into sections. The header section includes:
- DOCTYPE tag
- Meta tags
- Bootstrap CDN link
- Bootstrap Icons CDN link
- A custom stylesheet link pointing to `css/style.css`
- The latest Jquery CDN link
- Dynamic page title that needs to be set on every page

I recommend taking the Header, Navbar and Footer sections and put them in individual files inside the PHP includes directory.
This will allow you to only have to include these sections on each page rather than type all that for every page. Inside the Navbar section, there is some
PHP code that hides the Login and Sign Up buttons on the Navbar if the $_SESSION["loggedin"] variable is set and is true. If you dont know what this is or how to implement it just cut those sections out. They are on lines:

- 55-59
- 68-70
- 74-76

The footer section closes the `body` and `html` tags and also includes a link to the Bootstrap Javascript Files.
