---
title: OME Style Guide

toc_footers:


language_tabs:
  - scss

search: false
---

# General
```                                         
  ______             __  __                                                                 
 /      \           /  |/  |                                                                
/$$$$$$  | _______  $$ |$$/  _______    ______                                              
$$ |  $$ |/       \ $$ |/  |/       \  /      \                                             
$$ |  $$ |$$$$$$$  |$$ |$$ |$$$$$$$  |/$$$$$$  |                                            
$$ |  $$ |$$ |  $$ |$$ |$$ |$$ |  $$ |$$    $$ |                                            
$$ \__$$ |$$ |  $$ |$$ |$$ |$$ |  $$ |$$$$$$$$/                                             
$$    $$/ $$ |  $$ |$$ |$$ |$$ |  $$ |$$       |                                            
 $$$$$$/  $$/   $$/ $$/ $$/ $$/   $$/  $$$$$$$/                                             

 __       __                          __                                                    
/  \     /  |                        /  |                                                   
$$  \   /$$ |  ______   _____  ____  $$ |____    ______    ______                           
$$$  \ /$$$ | /      \ /     \/    \ $$      \  /      \  /      \                          
$$$$  /$$$$ |/$$$$$$  |$$$$$$ $$$$  |$$$$$$$  |/$$$$$$  |/$$$$$$  |                         
$$ $$ $$/$$ |$$    $$ |$$ | $$ | $$ |$$ |  $$ |$$    $$ |$$ |  $$/                          
$$ |$$$/ $$ |$$$$$$$$/ $$ | $$ | $$ |$$ |__$$ |$$$$$$$$/ $$ |                               
$$ | $/  $$ |$$       |$$ | $$ | $$ |$$    $$/ $$       |$$ |                               
$$/      $$/  $$$$$$$/ $$/  $$/  $$/ $$$$$$$/   $$$$$$$/ $$/                                

 ________                                __  __                                      __     
/        |                              /  |/  |                                    /  |    
$$$$$$$$/  _______    ______    ______  $$ |$$ | _____  ____    ______   _______   _$$ |_   
$$ |__    /       \  /      \  /      \ $$ |$$ |/     \/    \  /      \ /       \ / $$   |  
$$    |   $$$$$$$  |/$$$$$$  |/$$$$$$  |$$ |$$ |$$$$$$ $$$$  |/$$$$$$  |$$$$$$$  |$$$$$$/   
$$$$$/    $$ |  $$ |$$ |  $$/ $$ |  $$ |$$ |$$ |$$ | $$ | $$ |$$    $$ |$$ |  $$ |  $$ | __
$$ |_____ $$ |  $$ |$$ |      $$ \__$$ |$$ |$$ |$$ | $$ | $$ |$$$$$$$$/ $$ |  $$ |  $$ |/  |
$$       |$$ |  $$ |$$ |      $$    $$/ $$ |$$ |$$ | $$ | $$ |$$       |$$ |  $$ |  $$  $$/
$$$$$$$$/ $$/   $$/ $$/        $$$$$$/  $$/ $$/ $$/  $$/  $$/  $$$$$$$/ $$/   $$/    $$$$/  
```


![alt text](/images/screenshot.png)

Style guide for the Online Member Enrollment project.


## Grid

The design is based off of a 12 column grid.

![alt text](/images/grid.png)

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

// Green
$g300: #288837;

// Neutral
$n600: #4a4d56;
$n500: #85868C;
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

.gershwin {
  background: $g200;
  background-image: linear-gradient(-180deg, rgba(255,255,255,0.00) 0%, rgba(216,219,226,0.40) 100%);
}
```
The color scheme is organized by Color, Neutral or Gray and from darkest to lightest.

![alt text](/images/color.png)

## Typography

```scss
  $book   : 400;
  $medium : 500;
  $bold   : 600;
  $black  : 700;
```

The primary typeface used for OME is Circular. The four font weights are book, medium, bold and black.

## Assets

```
// Default Credit Card SVG
<svg width="34px" height="22px" viewBox="0 0 34 22" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
    <desc>Created with Sketch.</desc>
    <defs></defs>
    <g id="Symbols" stroke="none" stroke-width="1" fill="none" fill-rule="evenodd">
        <g id="component/desktop/payment/pay-with-card" transform="translate(-9.000000, -122.000000)">
            <g id="component/payment/pay-with-card">
                <g id="input-number" transform="translate(0.000000, 100.000000)">
                    <g id="fake-cc" transform="translate(9.000000, 22.000000)">
                        <rect id="card-bg" fill="#CECECE" x="0" y="0" width="34" height="21.4590164" rx="2"></rect>
                        <g id="group-number-bar" transform="translate(3.000000, 15.000000)" fill="#A7A7A7">
                            <rect id="number-bar-1" x="1.78e-14" y="0" width="6.13114754" height="1.67213115"></rect>
                            <rect id="number-bar-2" x="7.13661202" y="0" width="6.13114754" height="1.67213115"></rect>
                            <rect id="number-bar-3" x="14.273224" y="0" width="6.13114754" height="1.67213115"></rect>
                            <rect id="number-bar-4" x="21.4098361" y="0" width="6.13114754" height="1.67213115"></rect>
                        </g>
                        <rect id="white-box" fill="#FAFAFA" x="3" y="6" width="8" height="5" rx="1"></rect>
                    </g>
                </g>
            </g>
        </g>
    </g>
</svg>
```

* Credit Card SVGs -  https://muffinresearch.co.uk/svg-credit-card-icons/
* Default Card SVGs - See sample code
* Country Flag SVGs - http://flag-icon-css.lip.is/
* Icon SVGs - feathericons.com

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

**Behaviors & Examples**

* These buttons are used for the most important action on the screen.
* Hover: background color changes to darker blue
* Example: Continue button on each application section

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
    background: $g200;
  }
}
```

![alt text](/images/elements/button-secondary.png)

**Behaviors & Examples**

* These buttons are used for the second most important action on the screen.
* Hover: background color changes to slight gray
* Example: Back or Cancel button on each application section

## Button - Tertiary

```scss
// Upload Button
.button {  
  color: $g700;
  background: $n300;
  font-size: 13px;
  font-weight: 600;
  letter-spacing: 0.4;
  text-transform: uppercase;
  padding: 12px 24px;
  border-radius: 2px;

  &:hover {
    border: 1px solid $n400;
  }
}
```

![alt text](/images/elements/buttonupload.png)

**Behaviors:**

* Tertiary buttons are used as the upload button
* There are several states: Default, Hover, In Progress, Successful, Error
* Default: the normal resting state
* Hover: the border changes to a darker gray
* In Progress: replaces the text with a spinning icon
* Successful: replaces the spinning icon with a checkmark and word 'successful'
* Error: replace the spinning icon with error text


**Example:**

* Upload Document in Tax section

## Button - Option

```scss
// Tertiary Button
.button {  
  color: $g800;
  font-size: 15px;
  font-weight: 400;
  padding: 14px 24px;
  background: $n200;
  background-image: linear-gradient(-180deg,
                    rgba(255,255,255,0.00) 0%,
                    rgba(216,219,226,0.40) 100%);
  border: 1px solid $n400;
  border-radius: 2px;

  &:hover {
    background-image: linear-gradient(-180deg,
                      rgba(255,255,255,0.00) 0%,
                      rgba(17,120,206,0.04) 100%);
    border: 1px solid #1178CE;
    background-color: $g100;
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
* Example: user selects billing address

## Button Group

```scss
.button-group {
  margin-top: 60px;
  margin-bottom: 36px;
}

.button:first-child {
  margin-right: 12px;
}
```

![alt text](/images/elements/buttongroup.png)

**Behaviors:**

* This group with a primary and secondary button is separated by 12px
* This group is used at the end of each application section
* Secondary button is first in order, Primary button is second in order.


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

a::hover {
  color: $b600;
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

![alt text](/images/elements/anchorlinks.png)

**Behaviors:**

* Hover: the text, underline and icon change to a darker blue
* Default: contain a bottom border thats 5px below the baseline
* Contains Icon: 8px of space between icon and text, no border on hover
* Examople: Links in tax section and adding a new address in Royalties section

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
* Example: User adding their name, address, tax ID, etc


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
* Example: Selecting a genre

## Checkboxes

![alt text](/images/elements/checkbox.png)

**Behaviors:**

* Checkboxes are used when users need to make a selection
* There are two states: Default and Selected
* Default: the box only has an outline and the center is white
* Selected: the box background becomes blue with a white checkmark icon in the center
* Example: Option to enroll in direct deposit

## Radio Buttons

![alt text](/images/elements/radiobutton.png)

**Behaviors:**

* Radio buttons are used when users need to make a single selection out of a couple options
* There are two states: Default and Selected
* Default: the circle only has an outline and the center is white
* Selected: the circles background becomes blue with a white smaller circle in the middle
* Example: Agree to terms and conditions

## Labels & Descriptions

```scss
.label {
  font-size: 16px;
  line-height: 20px;
  font-weight: $medium;
  color: $g800;
  margin-bottom: 1px;
}

.description {
  font-size: 13px;
  line-height: 20px;
  font-weight: $book;
  color: $g800;
  opacity: 0.74;
  margin-bottom: 18px;
}
```

![alt text](/images/elements/labeldescription.png)

**Behaviors:**

* Labels are used to identify a form group, such as asking for a name
* Descriptions are used to give the user context for the form group
* The spacing between the title and description is 1px
* The spacing after the description and first form element is 18px
* Example: Asking users for their full name in General Section

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
* Example Default: Required documents or account creation Components
* Example Floating: Donation component

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
* Instagram
* Facebook
* Twitter

# Components

## Header

```scss
.site-title {
  font-size: 24px;
  font-weight: 400;
}

.app-title {
  color: $g100;
  font-size: 13px;
  font-weight: 600;
  letter-spacing: 1px;
  text-transform: uppercase;
}

.looking-for-help {
  color: $white;
  font-weight: 500;
  font-size: 16px;
  pading: 12px 24px;
  border: 2px solid $g100;
  border-radius: 2px;
}
```

![alt text](/images/components/header-writer.png)

**Behavior:**

* The header has 64px left/right padding and has a fixed position at the top of the browser window. The logo, titles and help link should be aligned center.
* Logo: Has a width of 104px and is positioned 26px from the top.
* App Title: The application title should reflect the application the user selects.
* Help Link: Clicking on this displays the Support Panel

## Footer

```scss
.footer {
  padding: 24px;
  border-top: 1px solid $n300;
}

.nav {
  font-weight: $medium;
  font-size: 12px;
  text-transform: uppercase;
  letter-spacing: 1px;
  margin-right: 24px;

  &:last-child {
    margin-right: 0;
  }
}

.nav-group {
  margin-bottom: 16px;
}

.social-icon-background {
  width: 32px;
  height: 32px;
  background: transparent;
}
```

![alt text](/images/components/footer.png)

**Behaviors:**

* Footer has 24px paddin with a 1px top border
* Navigation links are separated by 24px padding
* There's a 16px margin that separates the navigation and social icons
* Social Icons: have a size of 32x32
* Instagram: width of 18px
* Facebook: width of 8px
* Twitter: width of 18px

## Indicators

```scss
.circle {
  width: 25px;
  height: 25px;
  border-radius: 100%;
  background: $n400;
  margin-bottom: 6px;

  &--current {
    background: $b400;
  }

  &--completed {
    background-color: $b600;
  }
}

.section-title {
  color: $g800;

  &--inactive {
    color: $n400;
  }
}
```

![alt text](/images/components/indicator.png)

**Behaviors:**

* Indicators are used to show the user where they are currently in the application process and the next steps
* Indicator circles change color and icon depending on completion of sections.

## Application Sections

![alt text](/images/components/formsection.png)

**Behaviors:**

* A form section is comprised of a label, description, cards and form elements (inputs, dropdowns, etc)
* The spacing between the form title and first form group is 24px.
* The spacing between the last form group and button groups is 60px
* The spacing between the button groups and next form title is 36px

**Sections:**

* Indicators with section titles
* Form Groups
* Button Group - Continue and Back buttons

## Form Group

![alt text](/images/elements/formgroup.png)

**Behaviors:**

* A form group is comprised of a label, description and form elements (inputs, dropdowns, etc)
* The spacing between form elements is 14px
* The spacing between the description and first form element is 18px
* The spacing after the form group is 36px on desktop and 24px on mobile

**Example:**

* Resident Address in General Section

## Tooltips
```scss
.tooltip {
  padding: 12px;
  box-shadow: 0 2px 4px 0 rgba(13,13,13,0.40);
  background: $g700;
  border-radius: 6px;
}
````

![alt text](/images/components/tooltip.png)

**Behaviors:**

* Tooltips appear when someone hovers or clicks on the tooltip icon (circle with ?)
* Tooltips have 12px padding and a border radius of 6px
* Example: CVC Tooltip and Bank Routing/Account Number Tooltip

## Donation

![alt text](/images/components/donation.png)

**Behaviors:**

* The donation component uses the Floating Card style
* When a user selects the 'other' option, the card expands to display the additional fields (donation amount, Required information)

## Payment Summary

![alt text](/images/components/paymentsummary.png)

**Behaviors:**

* This displays the application fee and donation amounts
* The sum is displayed at the bottom

## Membership Options

```scss

// Header: writer, publisher, both
font-weight: $medium;
color: $g700;
font-size: 16px;
padding:14px 18px;

// Membership Pricing
font-weight: $book;
color: $b600;
font-size: 48px;

// The $ beside price
font-size: 16px;

// Application Fee
font-weight: $bold;
color: $b600;
font-size: 12px;
letter-spacing: 0.6px;
text-transform: uppercase;

// non-refundable
font-size: 11px;
font-weight: $book;
color: $n500;

// Body Copy
font-size: 13px;
line-height: 20px;
font-weight: $book;

// Requirements
font-weight: $medium;
font-size: 13px;

// Requirements List
line-height: 32px;
font-size: 13px;
font-weight: $book;
```

![alt text](/images/components/membershipoptions.png)

**Behaviors:**

* Three options are presented to the user in the Membership Selection section: Writer, Publisher, Both
* If the user selects publisher or both, a dropdown field appears below where they can select their publisher type

## Direct Deposit

![alt text](/images/components/directdeposit.png)

**Behaviors:**

* Direct Deposit component uses the Floating Card styling
* This only displays once the user checks the checkbox

## Create Account

![alt text](/images/components/createaccount.png)

**Behaviors:**

* Users can check if the username they entered in is available. Depending on outcome, a success/unavailable message displays below the input field
* When clicking 'check availability', the text changes to the loading icon
* When a user enters an invalid or non-matching password, an error message displays below the second input for password

## Required Documents

![alt text](/images/components/requireddocuments.png)

**Behaviors:**

* Required documents will display the sections (A, B, C, D) that are required depending on the users information
* Users are able to skip this section if they'd like
* If a user clicks on 'or add comment', the button and link are replaced with a textarea for the user to leave a comment

## Verify Address

![alt text](/images/components/verifyaddress.png)

**Behaviors:**

* Users must verify address and this modal appears.

## Verify Date of Birth

![alt text](/images/components/verifydateofbirth.png)

**Behaviors:**

* This modal appears to let users must verify their date of birth

## Add Address

![alt text](/images/components/addaddress.png)

**Behaviors:**

* User checks the checkbox and a card appears for the user to input their information and save the address. Once clicking save, the card becomes an option for the user to select.

## Support Panel

![alt text](/images/components/supportpanel.png)

**Behaviors:**

* This panel has two views: The question view, where it lists all the questions and the answer view, where it lists the answer to the question selected.
* At the bottom of every answer is a 'was this helpful' questions with the options to select yes or no.
