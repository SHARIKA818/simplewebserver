# EX01 Developing a Simple Webserver
## Date:

## AIM:
To develop a simple webserver to serve html pages.

## DESIGN STEPS:
### Step 1: 
HTML content creation.

### Step 2:
Design of webserver workflow.

### Step 3:
Implementation using Python code.

### Step 4:
Serving the HTML pages.

### Step 5:
Testing the webserver.

## PROGRAM:

```
<!DOCTYPE html>
<html lang="en">
<head>
    <title>FORMULA1</title>
    <style>
        a:hover{
            color: gray;
        }
        a{
            padding: 10px;
            font-size: 20px;
            text-decoration: none;
            font-family: Verdana;
        }
        ::placeholder
        {
          font-family: 'Times New Roman';
          font-size: 30px;
          font-style: initial;
          text-align: center;
        }
        input[type="submit"]:hover
        {
            border-width: 3px;
            border-color: black;
            background-color: gray;
        }
        input[type="text"]
        {
            border-radius: 25px;
            background-color :black;
        }
        h1{
          font-family: Tahoma;
          color: crimson;
          border-color: black;
        }
        
    </style>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" crossorigin="anonymous">
</head>
<body  bgcolor="gray">
    
        <div style="display: flex;">
            <div >
                <img src="ff1.jpg" alt="" height="200px">
            </div>
            <div >
                <a href="traf.html" style="color: red;text-decoration: none;font-family: Verdana;">speedscape</a>
                <a href="Zoro.html" style="color: red;text-decoration: none;font-family: Verdana;">Mercedes</a>
                <a href="Tab.html" style="color: red;text-decoration: none;font-family: Verdana;">Ferrari</a>
                <a href="rengo.html" style="color: red;text-decoration: none;font-family: Verdana;padding-right: 30px;">F1 2024</a>
                <input type="text" name="sear" style="border-radius: 20px;border-color: black;width: 200px;height: 40px;background-image: url(see.png);background-size: contain;
                background-repeat: no-repeat;background-position: 2%;text-align: center;font-size: 30px;border: 5px solid black;" placeholder="Search">
                <input type="submit" class="se" name="sub" value="Go">
                
            </div>
            <div>
                <img src="ff2.jpg" alt="" height="150px" style="padding-left: 200px;">
            </div>
        </div><br>
        <center>
        <h1 style="font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; font-style: italic;font-size: 50px;color: black;background-color: royalblue;">RACING THROUGH THE WORLD OF FORMULA 1</h1>
      </center>
        <div id="carouselExampleIndicators" class="carousel slide">
            <div class="carousel-indicators">
              <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
              <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1" aria-label="Slide 2"></button>
              <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="2" aria-label="Slide 3"></button>
            </div>
            <div class="carousel-inner">
              <div class="carousel-item active">
                <img src="ff333.jpg" class="d-block w-100" alt="..." height="800px">
              </div>
              <div class="carousel-item">
                <img src="ff4.jpg" class="d-block w-100" alt="..." height="800px">
              </div>
              <div class="carousel-item">
                <img src="ff5.jpg" class="d-block w-100" alt="..." height="800px">
              </div>
            </div>
            <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="prev">
              <span class="carousel-control-prev-icon" aria-hidden="true"></span>
              <span class="visually-hidden">Previous</span>
            </button>
            <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="next">
              <span class="carousel-control-next-icon" aria-hidden="true"></span>
              <span class="visually-hidden">Next</span>
            </button>
            <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-YvpcrYf0tY3lHB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz" crossorigin="anonymous"></script>
          </div>
          <div style="display: flex;">
            <div class="card" style="width: 18rem;margin: 10px;">
              <img src="ff10.jpg" class="card-img-top" alt="..." height="150px">
              <div class="card-body">
                <h5 class="card-title">WHEELS</h5>
                <p class="card-text">On average, they can reach 185 miles per hour (m.p.h.). The fastest speed recorded so far for an F1 is 223.5 m.p.h. They are also known for their quick acceleration. Formula One cars can start at 0 m.p.h., reach 100 m.p.h., and come to a complete stop again in less than five seconds.</p>
                <a href="https://onepiece.fandom.com/wiki/Straw_Hat_Pirates?so=search" class="btn btn-primary">More</a>
              </div>
            </div>
            <div class="card" style="width: 18rem;margin: 10px;">
              <img src="ff7.jpg" class="card-img-top" alt="..." height="150px">
              <div class="card-body">
                <h5 class="card-title">FORMULA 1</h5>
                <p class="card-text">Formula 1 is a team sport. It needs to be to change all 4 tyres on a car in under 2 seconds! F1 teams design and build their cars and get them ready to race. Each has their own history. Each has their own unique approach. All want to be the fastest. But who should you root for?</p>
                <a href="https://onepiece.fandom.com/wiki/Heart_Pirates" class="btn btn-primary">More</a>
              </div>
            </div>
            <div class="card" style="width: 18rem;margin: 10px;">
              <img src="ff33.jpg" class="card-img-top" alt="..." height="150px">
              <div class="card-body">
                <h5 class="card-title">CLASS OF 2024</h5>
                <p class="card-text">Max Verstappen, Red Bull Racing RB19, Charles Leclerc, Ferrari SF-23, Oscar Piastri, McLaren MCL60, Lando Norris, McLaren MCL60, George Russell, Mercedes F1 W14, the rest of the field at the start.</p>
                <a href="https://onepiece.fandom.com/wiki/Red_Hair_Pirates" class="btn btn-primary">More</a>
              </div>
            </div>
            <div class="card" style="width: 18rem;margin: 10px;">
              <img src="ff9.jpg" class="card-img-top" alt="..." height="150px">
              <div class="card-body">
                <h5 class="card-title">FERRARI SQUAD</h5>
                <p class="card-text">How many Ferrari fans are there?
                    The United States represents the sixth largest market for Formula One in our analysis, with an estimated 12 million fans. Our data shows roughly a quarter of these fans support Ferrari (24%), a photo-finish ahead of McLaren and Red Bull Racing, which both have 22%.</p>
                <a href="https://onepiece.fandom.com/wiki/Kid_Pirates?so=search" class="btn btn-primary">More</a>
              </div>
            </div>
          </div>
            
          
    
</body>
</html>
```


## OUTPUT:

![alt text](<Screenshot (1).png>)

![alt text](<Screenshot (2).png>)

![alt text](<Screenshot (3).png>)


## RESULT:
The program for implementing simple webserver is executed successfully.
