# Dotter's Website

# Style
## All Elements
**Attribute:** *

**Type:** Default

**Description**:

    Default styling.

**Style:**
* Margin: 0
* Padding: 0

## Body
**Attribute:** body

**Type:** Default

**Description**:

    Default styling for body.

**Style:**
* Max width: 100%
* Width: 100vw
* Height: 100vh
* Background: #C9C4A9

## Header
**Attribute:** #l-header

**Type:** Layout

**Description:**

    This is the header for the website.

**Style:**
* Width: 100vw
* Max width: 100%
* Display: fixed
* Top: 0
* Left: 0
* Height: 120px;
* Background: #4E115C

## Content
**Attribute:** #l-content

**Type:** Layout

**Description:**

    This is where the content will reside.

**Style:**
* Margin
    * Top: [Size of header + 5]
    * Left: 10vw
    * Right: 10vw

**Children:**
* Section
* Clear Section

### Section
**Attribute:** .section

**Type:** Component

**Description:**

    This is going to contain a section of content.

**Style:**
* Margin:
    * Bottom: 30x
* Box Shadows:
    * Dark Layer 1:
        * X,Y: [0,5]
        * Blur: 5
        * Opacity: 30%
        * Colour: #171622
    * Dark Layer 2:
        * X,Y: [3,10]
        * Blur: 10
        * Opacity: 20%
        * Colour: #171622
    * Dark Layer 3:
        * X,Y: [5,20]
        * Blur: 20
        * Opacity: 30%
        * Colour: #171622
    * Light Layer 1:
        * X,Y: [0,-5]
        * Blur: 5
        * Opacity: 30%
        * Colour: #F4F3ED
    * Light Layer 2:
        * X,Y: [-3,-10]
        * Blur: 10
        * Opacity: 20%
        * Colour: #F4F3ED
    * Light Layer 3:
        * X,Y: [-5,-20]
        * Blur: 20
        * Opacity: 30%
        * Colour: #F4F3ED
* Background: #F2F0E5
* Border Radius: 15px
* `> *`:
    * `:not(:last-child)`:
        * Padding:
            * Bottom: 10px
    * `:last-child`:
        * Margin:
            * Bottom: 20px

**Children:**
* Image
* Text
* 3 column grid
* Button
* Divider
* Code block

#### Image
**Attribute:** .e-image

**Type:** Element

**Description:**

    Image element

**Style:**
* Object fit: cover
* Padding:
    * Left: 5px
    * Right: 5px

#### Image Cover
**Attribute:** .e-image .e-image--cover

**Type:** Modifier

**Description:**

    Image element modifier. Covers the left ar right edges

**Style:**
* Padding:
    * Left: 0
    * Right: 0

#### Text
**Attribute:** .e-text

**Type:** Element

**Description:**

    Text element

**Style:**
* Padding:
    * Left: 5px
    * Right: 5px

#### Code Block
**Attribute:** .e-code

**Type:** Element

**Description:**

    Code block element. Applies Highligh.js to contents.

**Style:**
* Padding:
    * Left: 5px
    * Right: 5px

#### Button
**Attribute:** .e-button

**Type:** Element

**Description:**

    Button element

**Style:**
* Margin:
    * Left: 5px
    * Right: 5px
* Padding: `3px 5px`
* Border: solid black 2px
* Width: fit-content
* Background: #EAD0F0

#### Important Button
**Attribute:** .e-button .e-button-highlight

**Type:** Modifier

**Description:**

    Button element modifier. Makes button more visible

**Style:**
* Background: #F5D178

#### Clear Button
**Attribute:** .e-button .e-button-clear

**Type:** Modifier

**Description:**

    Button element modifier. Makes button less visible

**Style:**
* Background: none

#### Divider
**Attribute:** .e-divider

**Type:** Element

**Description:**

    Divider element

**Style:**
* Height: 0
* Margin: `5px 10% 10px`
* Border: 1px #727272
* Width: fit-content


#### Grid
**Attribute:** .e-grid

**Type:** Element

**Description:**

    Grid element.

**Style:**
* Display: grid
* Grid template columns: `1fr 1fr 1fr`
* Grid gap: `2vh 2vw`
* Align items: start
* Padding:
    * Left: 5px
    * Right: 5px

### Clear Section
**Attribute:** .section .section--clear

**Type:** Modifier

**Description:**

    Modifies `section` component

**Style:**
* Margin:
    * Bottom: 30x
* Border Radius: 15px
