## Learning Objectives

* Frontend and Backend Development
* HTML, CSS, & Javascript
* Creating a Website/UI

## Frontend and Backend Development

Frontend and Backend are two most popular terms used in web development. These terms are very crucial for web development but are quite different from each other. Each side needs to communicate and operate effectively with the other as a single unit to improve the website’s functionality.

Languages used for front end are HTML, CSS, Javascript while those used for backend include Java, Ruby, Python, .Net.





![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_23990786469b4efda69eba14ac274140.png)



### Frontend

The part of a website that user interacts with directly is termed as front end.

It is also referred to as the ‘client side’ of the application.

It includes everything that users experience directly: text colors and styles, images, graphs and tables, buttons, colors, and navigation menu.

User Interface (UI) development is the part of Frontend development.

## HTML, CSS & Javascript

HyperText Markup Language (HTML), Cascading Style Sheets (CSS), and JavaScript are the languages that run the web. They’re very closely related, but they’re also designed for very specific tasks.
* HTML provides the basic structure of sites, which is enhanced and modified by other technologies like CSS and JavaScript.
* CSS is used to control presentation, formatting, and layout.
* JavaScript is used to control the behavior of different elements.



![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_88e86cd87e104a5c8656cf32251b7b2c.png)




Let’s understand this with a simple analogy.
* HTML is the bare bones that give a structure to our body.
* Javascript is the vessels that enable blood flow and thus help our body function.
* CSS is just our appearance.







![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_42e98c2a97744234ac12f44936ca1a03.png)






These concepts are actually the building blocks of web development. 

In the tutorial, understanding a basic overview of ‘what elements are performing which function’ will be sufficient.

However, if you wish to learn these concepts properly, you can go through the free resource here: https://www.w3schools.com/html/html_intro.asp

### The directory structure
As a refresher, this is the folder structure for our application:

webapp/  
├── server/  
│ ├── artifacts/  
│ │ ├── banglore_home_prices_model.pickle  
│ │ └── columns.json  
│ ├── server.py  
│ └── util.py  
├── client/  
│ ├── app.html  
│ ├── app.css  
│ └── app.js  
└── model/  
└── model.ipynb

We previously worked with the server folder. Now, we’ll be working with the client folder.

You’ll find all the files that’ll be used in the tutorial here: https://github.com/dphi-official/Micro-Courses/tree/master/Introduction_Model_Deployment/client

## Creating a Website/UI







<iframe width="560" height="315" src="https://www.youtube.com/embed/rD2xumR98w8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>






## Integrating Frontend and Backend

Till now, what all has been implemented is: You need to run the server.py file using python server.py but it doesn’t run your frontend automatically. The HTML File needs to be opened separately for that purpose.

Now, we’ll be making some changes such that on running the Flask application, our website runs automatically.

In the HTML File, the 6th and 7th lines are changed to

```
<script src="{{ url_for('static',filename='app.js') }}"></script>
  <link rel="stylesheet" href= "{{ url_for('static',filename='app.css') }}">
```

Next, we’ll be linking the Flask application to the frontend files.

We’ll simply edit the creating the Flask app line in the server.py file for this purpose:
In the server.py File, the 4th line is changed to
`app = Flask( name , static_url_path="/client", static_folder='../client', template_folder="../client")`

And that’s it!

You should now be able to run your application locally at http://127.0.0.1:5000 and it would look something like this:



![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_078c5352dd4e47afac0b1f9b274b008a.png)

### What Next?

Please note: CSS and Javascript are optional elements for creating a website. You could’ve just created a bare form that takes in input and prints an output as well.

So now that you are able to use your website, why not make it available to the world so that anyone and everyone can use it? That’s what we will cover in the last unit of this course.

### References

* https://www.geeksforgeeks.org/frontend-vs-backend/

### Slide Download Link

You can download the slides for this unit from [here](https://docs.google.com/presentation/d/1YmPfv86Yo4N7WU_MjyvrJ6ktvJmY4VM12EQR_ax5pRQ/edit?usp=sharing).