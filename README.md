# Foundation 5 - Kitchen Sink Snippets

A collection of snippets for easily creating ZURB Foundation 5 elements.

## Installing

  `cd ~/Library/Application\ Support/Sublime\ Text\ 2/Packages`
  `git clone git@github.com:kjbrum/foundation-5-kitchen-sink-snippets.git`
  
## Layout & Grid

### `zf-c` - create a container

    <div class="container">
    </div>

### `zf-r` - create a row

    <div class="row">
    </div>

### `zf-cr` - create a container and row

    <div class="container">
      <div class="row">
      </div>
    </div>

### `zf-col` - create a column

  <div class="small-[1-12] large-[1-12] column">
  </div>

### `zf-block-grid` - create a container and row

  <ul class="small-block-grid-[1-12] large-block-grid-[1-12]">
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
  </ul>

##  Buttons

### `zf-btn` - create a button

  <a href="#" class="[tiny small large] [secondary success alert] [radius round] button">Button</a>

### `zf-btn-group` - create a button group

  <ul class="[radius round] button-group">
    <li><a href="#" class="button">Button 1</a></li>
    <li><a href="#" class="button">Button 2</a></li>
    <li><a href="#" class="button">Button 3</a></li>
  </ul>

### `zf-btn-split` - create a button split

  <a href="#" class="[tiny small medium large] [radius round] button split">Split Button<span data-dropdown="drop"></span></a><br>
  <ul id="drop" class="f-dropdown" data-dropdown-content>
    <li><a href="#">Link 1</a></li>
    <li><a href="#">Link 2</a></li>
    <li><a href="#">Link 3</a></li>
  </ul>

### `zf-btn-dropdown` - create a button dropdown

  <a href="#" data-dropdown="drop" class="[tiny small medium large] [radius round] button dropdown">Dropdown Button</a><br>
  <ul id="drop" data-dropdown-content class="f-dropdown">
    <li><a href="#">Link 1</a></li>
    <li><a href="#">Link 2</a></li>
    <li><a href="#">Link 3</a></li>
  </ul>

### `zf-btn-bar` - create a button bar

  <div class="button-bar">
    <ul class="[radius round] button-group">
      <li><a href="#" class="button">Button 1</a></li>
      <li><a href="#" class="button">Button 2</a></li>
      <li><a href="#" class="button">Button 3</a></li>
    </ul>
    <ul class="[radius round] button-group">
      <li><a href="#" class="button">Button 1</a></li>
      <li><a href="#" class="button">Button 2</a></li>
      <li><a href="#" class="button">Button 3</a></li>
    </ul>
  </div>

## Credit
Inspiration from - https://github.com/zurb/foundation-5-sublime-snippets