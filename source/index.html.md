---
title: OME Style Guide

toc_footers:


language_tabs:
  - scss

search: false
---

# General

![alt text](/images/screenshot.png)

Style guide for the Online Member Enrollment project.


## Grid

The design is based off of a 12 column grid.

Title          | Mobile >599px   | Desktop <600px
-------------- | -------------- | --------------
Columns        | 1              | 12
Gutters        | 0px            | 16px (8px on left/right sides. No outside gutters)
Offset         | Left 56px      | Left 60px
Max-width      | 100%           | 720px
Margin         | 24px 16px      | 60px 36px

## Colors

```scss
// Blue
$b700: #002d5b;
$b600: #004183;
$b500: #175da7;
$b400: #1178ce;
$b300: #489CEF;

// Red
$r300: #cd35335;

// Neutral
$n600: #4a4d56;
$n400: #a9abb6;
$n300: #d8dbe2;
$n200: #eef0f5;
$n100: #f7f9fb;

// Grayscale
$g800: #0d0d0d;
$g700: #373737;
$g600: #6d6d6d;
$g400: #cecece;
$g200: #fafafa;
$g100: #ffffff;

// Gradients
.carnegie {
  background-image: linear-gradient(-135deg, $b500 0%, $b300 100%);
}

.beacon {
  background: $g100,
  background-image: linear-gradient(-180deg, rgba(255,255,255,0.00) 0%, $b400 3%)
}
```


![alt text](/images/color.png)

The color scheme is organized by Color, Neutral or Gray and from darkest to lightest.

## Typography

```scss
  $book   : 400;
  $medium : 500;
  $bold   : 600;
  $black  : 700;
```

Font Weights

# Elements

## Button - Primary

```scss
// Primary Button
.button {  
  color: $g100;
  background: $b400;
  font-size: 13px;
  font-weight: 600;
  letter-spacing: 0.4;
  text-transform: uppercase;
  padding: 12px 24px;
  border-radius: 2px;

  &:hover {
    background: $b500;
  }
}
```

![alt text](/images/elements/button-primary.png)

**Behaviors:**

* These buttons are used for the most important action on the screen.
* There is a hover state

**Example:**

* Continue button on each application section

## Button - Secondary

```scss
// Secondary Button
.button {  
  color: $g800;
  background: $g100;
  font-size: 13px;
  font-weight: 600;
  letter-spacing: 0.4;
  text-transform: uppercase;
  padding: 12px 24px;
  border-radius: 2px;

  &:hover {
    background: $b500;
  }
}
```

![alt text](/images/elements/button-secondary.png)

**Behaviors:**

* These buttons are used for the second most important action on the screen.
* There is a hover state

**Example:**

* Back or Cancel button on each application section

## Button - Tertiary

```scss
// Tertiary Button
.button {  
  color: $g800;
  font-size: 15px;
  font-weight: 400;
  padding: 14px 24px;
  text-transform: uppercase;
  background: #$n200;
  background-image: linear-gradient(-180deg,
                    rgba(255,255,255,0.00) 0%,
                    rgba(216,219,226,0.40) 100%);
  border: 1px solid $n400;
  border-radius: 2px;

  &:hover {
    background: $b500;
  }
}
```

![alt text](/images/elements/button-tertiary.png)

**Behaviors:**

* This button type is used for options within the application
* There are three states: Default, Hover and Active
* Default: the button displays in its normal, resting states
* Hover: the border changes color to a darker gray
* Active: the button's border and background-gradient changes to blue


**Example:**

* User selects billing address
* User selecting donation amount


## Button - Upload

```scss
// Upload Button
.button {  
  color: $g100;
  background: $n300;
  font-size: 13px;
  font-weight: 600;
  letter-spacing: 0.4;
  text-transform: uppercase;
  padding: 12px 24px;
  border-radius: 2px;

  &:hover {
    background: $b500;
  }
}
```

![alt text](/images/elements/button-upload.png)

**Behaviors:**

* This is the upload button so users can upload documents
* There are several states: Default, Hover, In Progress, Successful
* Default: the normal resting state
* Hover: the border changes to a darker gray
* In Progress: replaces the text with a spinning icons
* Successful: replaces the spinning icon with a checkmark and word 'successful'


**Example:**

* Upload Document in Tax section

## Button Group

![alt text](/images/elements/continue-and-back.png)

**Behaviors:**

* This group with a primary and secondary button is separated by 12px
* This group is used at the end of each application section
* Secondary button is first, Primary button is second.


## Anchor Links

```scss
a {
  color: $b500;
  font-weight: 500;
  font-size: 13px;
  line-height: 20px;

  &::before {
    content:'';
    width: 100%;
    height: 1px;
    color: $b500;
  }
}

a .has--icon-add {
  color: $b500;
  font-weight: 500;
  font-size: 15px;
  line-height: 24px;

  &::before {
    // svg of + icon
  }
}

```

![alt text](/images/elements/anchor-links.png)

**Behaviors:**

* Hover: the text, underline and icon change colors
* Default: contain a bottom border thats 5px below the baseline
* Contains Icon: 8px of space between icon and text, no border on hover


**Example:**

* Adding an Address in Royalties section
* Links in the Tax section

## Input

```scss
input {
  background: $g100;
  padding: 0 12px;
  height: 40PX;
  border: 1px solid $n500;
  border-radius: 2px;

  &::hover {
    border: 1px solid $n600;
  }

  &::active {
    border: 1px solid $b400;
  }

  &-fail {
    border: 1px solid $r300;
  }

  &-fail-description {
    font-size: 11px;
    color: $r300;
    line-height: 20px;
  }
}
```

![alt text](/images/elements/input.png)

**Behaviors:**

* Form inputs have a few states: Default, Hover, Active, Fail
* Hover: the border changes colors to a darker gray
* Active: the border changes colors to blue
* Fail: the border changes to red and an error message displays under the input

**Example:**

* User adding their name, address, tax ID, etc


## Dropdown

```scss
dropdown {
  background: $g100;
  padding: 0 12px;
  height: 40px;
  border: 1px solid $n500;
  border-radius: 2px;

  &::hover {
    border: 1px solid $n600;
  }

  &::active {
    border: 1px solid $b400;
  }

  .dropdown-option {
    background: $n200;  
  }
}
```

![alt text](/images/elements/dropdown.png)

**Behaviors:**

* Dropdowns have a few states: Default, Hover, Active, Fail
* Hover: the border changes colors to a darker gray
* Active: the border changes colors to blue and the menu expands showing options
* Fail: the border changes to red and an error message displays under the input

**Example:**

* Selecting a genre

## Checkboxes

![alt text](/images/elements/checkbox.png)

**Behaviors:**

* Checkboxes are used when users need to make a selection
* There are two states: Default and Selected
* Default: the box only has an outline and the center is white
* Selected: the box background becomes blue with a white checkmark icon in the center

**Example:**

* Option to enroll in direct deposit

## Radio Buttons

![alt text](/images/elements/radiobutton.png)

**Behaviors:**

* Radio buttons are used when users need to make a single selection out of a couple options
* There are two states: Default and Selected
* Default: the circle only has an outline and the center is white
* Selected: the circles background becomes blue with a white smaller circle in the middle

**Example:**

* Agree to terms and conditions

## Labels & Descriptions

```scss
.label {
  font-size: 16px;
  line-height: 20px;
  font-weight: $medium;
  color: $g800;
}

.description {
  font-size: 13px;
  line-height: 20px;
  font-weight: $book;
  color: $g800;
  opacity: 0.74;
}
```

![alt text](/images/elements/labeldescription.png)

**Behaviors:**

* Labels are used to identify a form group, such as asking for a name
* Descriptions are used to give the user context for the form group

**Example:**

* Asking users for their full name in General Section

## Cards

```scss
.card {
  background: $g200;
  padding: 24px 18px;
  border-radius: 2px;
  border: 1px solid $n300;

  &-floating {
    background: $n200;
    box-shadow: 0 2px 6px 0 rgba(13,13,13,0.10);
  }
}
```

![alt text](/images/elements/card.png)

**Behaviors:**

* Cards are used to identify sections of content
* There are two styles: default and Floating
* Default: used as a way to group content together
* Floating: used to display secondary actions after a primary action has taken place

**Example:**

* Default: Required documents or account creation Components
* floating: Donation component

## Icons

![alt text](/images/elements/icon.png)

**Behavior:**

* Icons are sized depending upon their context
* There are light and dark versions
* Light: the color is $g100
* Dark: the color is $g700
* The icons are taken from the open-source Feathericons.com

**Icon List:**

* Add
* Close
* Checkmark
* Loading
* Triangle
* Upload

# Components

## Header

The header has 64px left/right padding and has a fixed position at the top of the browser window. The logo, titles and help link should be aligned center.

### Logo

Has a width of 104px and is positioned 26px from the top.

### Site Title

```scss
  font-size: 24px;
  font-weight: 400;
```

### Application Title

The application title should reflect the application the user selects.

```scss
  color: $g100;
  font-size: 13px;
  font-weight: 600;
  letter-spacing: 1px;
  text-transform: uppercase;
```

### Help Link

```scss
  color: $white;
  font-weight: 500;
  font-size: 16px;
```


## Footer

## Indicators

![alt text](/images/components/indicator.png)

**Behaviors:**
* ...

## Application Sections

![alt text](/images/elements/formgroup.png)

**Behaviors:**

* A form group is comprised of a label, description and form elements (inputs, dropdowns, etc)
* The spacing between form elements is 14px
* The spacing between the description and first form element is 18px
* The spacing after the form group is 36px on desktop and 24px on mobile

**Sections:**

* Indicators with titles
* Form Groups
* Button Group - Continue and Back buttons

## From Group

![alt text](/images/elements/formgroup.png)

**Behaviors:**

* A form group is comprised of a label, description and form elements (inputs, dropdowns, etc)
* The spacing between form elements is 14px
* The spacing between the description and first form element is 18px
* The spacing after the form group is 36px on desktop and 24px on mobile

**Example:**

* Resident Address in General Section

# Animations
