![Screenshot (46)](https://github.com/user-attachments/assets/1a7d2ab9-5020-4bba-805d-c0ceef9cb81d)

'''
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Food Gallery</title>
    <style>
        body 
        {
            font-family: Arial, sans-serif;
        }

        .navbar h2
        {
            margin: 0;
            padding-left: 10px;
            font-size: 20px;
        }
        .navbar 
        {
            background-color: black;
            color: white;
            padding: 10px;
            text-align: right;
        }

        .navbar a 
        {
            color: white;
            margin: 0 5px;
            text-decoration: none;
        }

        .navbar a:hover 
        {
            text-decoration: underline;
            color: yellow;
        }

        .container 
        {
            text-align: center;
            margin: 20px auto;
        }

        .menu-title 
        {
            font-size: 24px;
            font-weight: bold;
            margin-bottom: 20px;
        }

        .gallery 
        {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
        }

        .menu-item 
        {
            width: 200px;
            border: 2px solid black;
            padding: 10px;
            background-color: #f4f405;
        }

        .menu-item img 
        {
            width: 100%;
            height: auto;
        }

        .menu-description 
        {
            font-size: 14px;
            margin-top: 10px;
        }

        .menu-item:hover .menu-description 
        {
            color: red;
            font-weight: bold;
        }

        .order-btn {
            display:flex;
            justify-content: center;
            align-items: center;
            margin: 0 auto;
            margin-top: 10px;
            width: 100px;
            height: 30px;
            padding: 10px 10px;
            background-color: black;
            color: white;
            text-decoration: none;
            border-radius: 25px;
        }

        .order-btn:hover {
            background-color: green;
        }

    </style>
</head>
<body>

    <div class="navbar">
        <h2 align="left">Mother's Kitchen</h2>
        <a href="#">Home</a>
        <a href="#">About Us</a>
        <a href="#">Special Menus</a>
        <a href="#">Contact Us</a>
    </div>

    <div class="container">
        <div class="menu-title">Special Menus</div>

        <div class="gallery">
            <div class="menu-item">
                <img src="data:image/jpeg;base64,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" alt="Food 1">
                <div class="menu-description">Lorem ipsum dolor sit amet consectetur adipisicing elit. Tempora, aut.</div>
            </div>

            <div class="menu-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQoE3yQ-PXA73a3nJYtR3sucAac0bWhe99ogcZK0sVpsfMwuON9LIqmAgnF4KzT1jftQp8&usqp=CAU" alt="Food 2">
                <div class="menu-description">Lorem ipsum dolor sit amet consectetur adipisicing elit. Tempora, aut.</div>
            </div>

            <div class="menu-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRYehX8pFtzwyooKMFQeyBTTACDwES347P4Xg&s" alt="Food 3">
                <div class="menu-description">Lorem ipsum dolor sit amet consectetur adipisicing elit. Tempora, aut.</div>
            </div>

            <div class="menu-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTA9h4EH1Iy-R_XhliioyfqTF5qEoPiTH3qxQ&s" alt="Food 4">
                <div class="menu-description">Lorem ipsum dolor sit amet consectetur adipisicing elit. Tempora, aut.</div>
            </div>
        </div>
    </div>
    <a href="#" class="order-btn" >Order here</a>


</body>
</html>
'''
