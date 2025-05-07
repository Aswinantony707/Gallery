# Ex.08 Design of Interactive Image Gallery
# Date:7-5-2025
# AIM:
To design a web application for an inteactive image gallery with minimum five images.

# DESIGN STEPS:
## Step 1:
Clone the github repository and create Django admin interface.

## Step 2:
Change settings.py file to allow request from all hosts.

## Step 3:
Use CSS for positioning and styling.

## Step 4:
Write JavaScript program for implementing interactivity.

## Step 5:
Validate the HTML and CSS code.

## Step 6:
Publish the website in the given URL.

# PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
   
    <body>
        <header>
            <h1><font color="black">Top 10 Best Pet Fish</font></h1>
        </header>
        <header>
            <h2><font color="black">for your aquarium </font></h2>
        </header>
    </body>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            text-align: center;
            background-color: #f4f4f478;
             background-image: url("anime\ world.webp");
            background-size:cover;
        }

        h1 {
            margin-top: 20px;
        }

        .gallery {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 15px;
            padding: 20px;
        }

        .gallery img {
            width: 300px;
            height: 200px;
            border: 2px solid #cccccc;
            border-radius: 8px;
            cursor: pointer;
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .gallery img:hover {
            transform: scale(1.1);
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.227);
        }

        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.8);
            justify-content: center;
            align-items: center;
            z-index: 1000;
        }

        .modal img {
            max-width: 90%;
            max-height: 90%;
            border: 4px solid white;
            border-radius: 10px;
        }

        .modal span {
            position: absolute;
            top: 20px;
            right: 40px;
            font-size: 30px;
            color: rgba(255, 255, 255, 0.526);
            cursor: pointer;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <h1>Interactive Photo Gallery</h1>
    <div class="gallery">
        <img src="aswin.png" alt="Image 1" onclick="openModal(this)">
        <img src="ers.png" alt="Image 2" onclick="openModal(this)">
        <img src="yig.png" alt="Image 3" onclick="openModal(this)">
        <img src="sra.png " alt="Image 4" onclick="openModal(this)">
        <img src=" fyfd.png      " alt="Image 5" onclick="openModal(this)">
        <img src="ewd.png   " alt="Image 5" onclick="openModal(this)">
        <img src="jg.png    " alt="Image 5" onclick="openModal(this)">
    </div>
    <div class="modal" id="imageModal">
        <span onclick="closeModal()">&times;</span>
        <img id="modalImage" src="" alt="">
    </div>
    <script>
        function openModal(image) {
            const modal = document.getElementById('imageModal');
            const modalImg = document.getElementById('modalImage');
            modal.style.display = 'flex';
            modalImg.src = image.src;
        }
        function closeModal() {
            const modal = document.getElementById('imageModal');
            modal.style.display = 'none';
        }
    </script>
</body>
</html>

```
# OUTPUT:
![Screenshot 2025-05-07 234140](https://github.com/user-attachments/assets/88102729-1f4c-4fb2-8b70-6b8c81fb5e1e)
![Screenshot 2025-05-07 234252](https://github.com/user-attachments/assets/74670be8-66e3-4598-a82c-c5b6dd27443a)
![Screenshot 2025-05-07 234150](https://github.com/user-attachments/assets/7325e2b1-6815-4709-b575-d870c05c08f2)
![Screenshot 2025-05-07 234207](https://github.com/user-attachments/assets/7cc4a10e-81b8-46af-9bab-5dc577e7d709)
![Screenshot 2025-05-07 234236](https://github.com/user-attachments/assets/6fbd64ca-9119-4aa3-84f7-347cc676e6fd)
![Screenshot 2025-05-07 234222](https://github.com/user-attachments/assets/22884bb1-17d3-44b7-9417-10f2201c1bbc)
# RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
