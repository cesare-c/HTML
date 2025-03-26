# Unit Conversion using HTML5 Structural Elements

## Task 1: Create the basic app structure, with inpage navigation

1. Create a new file named `index.html`.

```bash
touch index.html
```
2. Insert the basic HTML document structure

 ```html
 html:5
 ```
Change the title to `Unit Conversions`

3. Create a section with id` home`

```html
section#home
```


4. Within the home section, create a header, using the `<header>` tag, with the text `Unit Conversions`. `Bold` the text to make it stand out

```html
<section id="home">
    <!-- This is the main heading -->
    <header><b>Unit Conversions</b></header>
</section>
```

5. Create a navigation bar inside the home section, after the header tag

For Temperature, Weight, Distance:

- We will create anchor tags with buttons which redirect users to certain sections of the same page.

- We will be using the id attribute to reference these sections. ids are represented with the # symbol.

```html
<nav>
  <!-- Button for redirecting users to the temperature section -->
  <a href="#temperature"><button>Temperature</button></a>

  <!-- Button for redirecting users to the weight section -->
  <a href="#weight"><button>Weight</button></a>

  <!-- Button for redirecting users to the distance section -->
  <a href="#distance"><button>Distance</button></a>
</nav>
```

## Task 2: Create the `div` container for all 3 convesrion

```html
<div id="all-conversion-sections">
        <!-- section for Temperature -->
        <!-- section for Weight -->
        <!-- section for Distance -->
</div>
```

## Task 3: Temperature (Celsius to Fahrenheit) Conversion

1. Create a `<section>` with id `temperature`
2. Create a div tag with id set to `tmp`. Add a `figure` tag inside this div tag, where you will be adding a visual depiction of the conversion.
3. Add an `image `tag inside the figure, having `src` attribute set to the URL “https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-CD0101EN-SkillsNetwork/labs/Theia%20Labs/02%20-%20HTML5%20Elements/images/thermo.png“ and a width set to 200px. Then, add a figcaption tag to give a caption to this figure.

4. Next you will complete the following:
- Display temperature as a heading
- Create two input fields and two labels
- Create a button to convert

5. Add an aside tag after the article to teach a user how to do this calculation themselves.

```html
<section id="temperature">
            <!-- Temperature conversion section -->
            <div id="tmp">
                <figure>
                    <img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-CD0101EN-SkillsNetwork/labs/Theia%20Labs/02%20-%20HTML5%20Elements/images/thermo.png" width="200px"/>
                    <figcaption>Celsius to Fahrenheit Conversion</figcaption>
                </figure>
                <article>
                    <!-- This contains the specific elements for temperature conversion -->
                    <fieldset>
                        <legend>Temperature</legend>
                        <!-- Label for Temperature input -->
                        <label for="celsius">Celsius</label> <br/>
                        <input type="number" id="celsius"> <br/>
                      
                        <!-- The conversion button -->
                        <button id="temperature"> Convert </button> <br/>
                      
                        <!-- Label for Temperature output -->
                        <input type="number" id="fahrenheit"> <br/>
                        <label for="fahrenheit">Fahrenheit</label>
                    </fieldset>
                </article>
                <aside>
                    To convert celsuis to fahrenheit yourself, use this formula replacing the `C` with your temperature in celsuis: (C × 9/5) + 32
                </aside>
            </div>
        </section>
```

## Task 4: Weight (Kilograms to Pounds) Conversion

- similar with Task 3

## Task 5: Distance (Kilometers to Miles) Conversion

- similar with Task 3

## Task 6: Add the page footer and home button

1. Add another `div` tag, below the `all-conversion-sections div` with attribute id set to `go-home`, to navigate to the top of the page. Copy and paste the following code in the div, to render a button with a home icon.

```html
<div id="go-home">
    <a href="#home">
        <img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-CD0101EN-SkillsNetwork/labs/Theia%20Labs/02%20-%20HTML5%20Elements/images/home.svg"/>
    </a>
</div>
```

2. Add a `footer` tag inside the body tag, after the go-home div tag.

```html
<footer>Learn more about HTML as a part of the <a href="">IBM</a> Fullstack Web Developer Certification</footer>
```
