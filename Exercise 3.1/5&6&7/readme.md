![Screenshot (48)](https://github.com/user-attachments/assets/9b8b6a23-3eb1-4f09-8b45-5e7e47b7720e)
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Styled Table</title>
    <link href="..\css\style01.css" rel="stylesheet"> <!-- External CSS file link -->
</head>
<body>

    <h1>Student Data Table</h1>

    <table>
        <th>
            <tr>
                <th>Name</th>
                <th>Age</th>
                <th>Grade</th>
            </tr>
        </th>
            <tr>
                <td>Alice</td>
                <td>20</td>
                <td>A</td>
            </tr>
            <tr>
                <td>Bob</td>
                <td>21</td>
                <td>B</td>
            </tr>
            <tr>
                <td>Clara</td>
                <td>22</td>
                <td>A</td>
            </tr>
            <tr>
                <td>David</td>
                <td>23</td>
                <td>C</td>
            </tr>
            <tr>
                <td>Eve</td>
                <td>24</td>
                <td>B</td>
            </tr>
            <tr>
                <td>Frank</td>
                <td>25</td>
                <td>A</td>
            </tr>
            <tr>
                <td>Grace</td>
                <td>26</td>
                <td>B</td>
            </tr>
            <tr>
                <td>Henry</td>
                <td>27</td>
                <td>C</td>
            </tr>
            <tr>
                <td>Isabel</td>
                <td>28</td>
                <td>A</td>
            </tr>
            <tr>
                <td>John</td>
                <td>29</td>
                <td>B</td>
            </tr>
    </table>
    <h2>List of Links</h2>
    <ul id="links">
    <li>
    <a href="https://google.com">Hello</a>
    </li>
    <li>
    <a href="https://google.com">welcome</a>
    </li>
    <li>
    <a href="https://google.com">our_world</a>
    </li>
    </ul>
    <button class="custom-button">1</button>
    <button class="custom-button">2</button>
    <button class="custom-button">3</button>
    <button class="custom-button">4</button>
</body>
</html>
```

CSS :
```html
table {
    text-align: center;
    border: 2px solid black;
    border-collapse: collapse;
    width: 700px;
    height: 700px;
    }
    table th {
    border: 2px solid black;
    background-color: black;
    color: white;
    font-family: 'Times New Roman', Times, serif;
    
    }
    table tr:nth-child(odd) {
    background-color: greenyellow;
    }
    table tr:nth-child(even) {
    background-color: grey;
    }
    table, th, td {
        border: 3px solid black; 
    }
    
    #links a {
        text-decoration: none;
        font-style: italic;
        font-weight: bold;
        }
        #links li{
        list-style: circle;
        }
        #links a:link {
        color: blue; 
        }
        #links a:visited {
        color: purple; 
        }
        #links a:hover {
        color: rgb(41, 181, 34);
        }
        #links a:active {
        color: green;
        }
        .custom-button{
        height: 90px;
        width: 90px;
        background-color: rgb(99, 153, 235);
border-radius: 50%;
}
.custom-button:hover {
background-color: aqua;
}
```
