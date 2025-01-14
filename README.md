# flask-example

A minimal web app developed with [Flask](http://flask.pocoo.org/) framework. 

The main purpose is to introduce how to implement the essential elements in web application with Flask, including

- URL Building

- Authentication with Sessions

- Template & Template Inheritance

- Error Handling

- Integrating with *Bootstrap*

- Interaction with Database (SQLite)

- Invoking static resources

- Deploying in a Docker container server

For more basic knowledge of Flask, you can refer to [a tutorial on Tutorialspoint](https://www.tutorialspoint.com/flask/).

Further, we want to provide an example for how to deploy this website into production on the public web by offering a sample container.


## How to Run


- Step 1: Make sure you have Docker installed
 
- Step 2: Build and run the Docker container your favorite way, via VSCode (all necessary configuration files are included) or with  terminal commands. When you run the container, don't forget to publish port 8080 and run the server. This can be done like so, in the repository root, run: 

docker build . -t flask-example
docker run -p 8080:8080 flask-example python server.py

- Step 3: Visit the site at the port you published in your browser.

## Details about This Toy App

There are three tabs in this toy app

- **Public**: this is a page which can be accessed by anyone, no matter if the user has logged in or not.

- **Private**: Only logged-in user can access this page. Otherwise the user will get a 401 error page.

- **Admin Page**: This part is only open to the user who logged in as "Admin". In this tab, the administrator can manage accounts (list, delete, or add).


A few accounts were set for testing, like ***admin*** (password: admin), ***test*** (password: 123456), etc. You can also delete or add accounts after you log in as ***admin***.



## References

- http://flask.pocoo.org/

- https://www.tutorialspoint.com/flask/



## Credict
Image private.jpg: https://commons.wikimedia.org/wiki/File:(315-365)_Locked_(6149414678).jpg

Image public.jpg: https://commons.wikimedia.org/wiki/File:Drown%3F!_(131380682).jpg
