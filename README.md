# Ex.08 Design of Interactive Image Gallery
## Date: 09.05.2025
## AIM
  To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS

## Step 1:

Clone the github repository and create Django admin interface

## Step 2:

Change settings.py file to allow request from all hosts.

## Step 3:

Use CSS for positioning and styling.

## Step 4:

Write JavaScript program for implementing interactivit

## Step 5:

Validate the HTML and CSS code

## Step 6:

Publish the website in the given URL.

## PROGRAM
```
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Photo Gallery</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            text-align: center;
            background-image: url(https://static.vecteezy.com/system/resources/thumbnails/049/855/272/small/nature-background-high-resolution-wallpaper-for-a-serene-and-stunning-view-photo.jpg);
            background-size: cover;  
            background-position: center;
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
            height: 250px;
            border: 5px solid #080202;
            border-radius: 8px;
            cursor: pointer;
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .gallery img:hover {
            transform: scale(1.1);
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
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
            border: 4px solid rgb(9, 1, 1);
            border-radius: 10px;
        }

        .modal span {
            position: absolute;
            top: 20px;
            right: 40px;
            font-size: 30px;
            color: rgb(9, 4, 4);
            cursor: pointer;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <h1>Interactive Photo Gallery</h1>
    <div class="gallery">
        <img src="i1 (1).png" alt="Image 1">
        <img src="i1 (2).png" alt="Image 2">
        <img src="i1 (3).png" alt="Image 3">
        <img src="i1 (4).png" alt="Image 4">
        <img src="i1 (5).png" alt="Image 5">
        <img src="i1 (6).png" alt="Image 6">
        <img src="i1 (7).png" alt="Image 7">
        <img src="i1 (8).png" alt="Image 8">
        <img src="i1 (9).png" alt="Image 9">
        <img src="i1 (10).png" alt="Image 10">
        <img src="i1 (11).png" alt="Image 11">
        <img src="i1 (12).png" alt="Image 12">
        <img src="i1 (13).png" alt="Image 13">
        <img src="i1 (14).png" alt="Image 14">
        

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
## OUTPUT
![alt text](<Screenshot 2025-05-09 114101.png>)

## RESULT
  The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
