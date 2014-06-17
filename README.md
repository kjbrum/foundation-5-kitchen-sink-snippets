# Foundation 5 - Kitchen Sink Snippets

A collection of snippets for easily creating ZURB Foundation 5 elements.

## Installing

    cd ~/Library/Application\ Support/Sublime\ Text\ 2/Packages
    git clone git@github.com:kjbrum/foundation-5-kitchen-sink-snippets.git
  
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

    <div class="small-[1-12] medium-[1-12] large-[1-12] column">
    </div>

### `zf-block-grid` - create a container and row

    <ul class="small-block-grid-[1-12] medium-block-grid-[1-12] large-block-grid-[1-12]">
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

## Navigation

### `zf-off-canvas` - create an off-canvas block

    <div class="off-canvas-wrap">
      <div class="inner-wrap">
        <nav class="tab-bar">
          <section class="left-small">
            <a class="left-off-canvas-toggle menu-icon" ><span></span></a>
          </section>

          <section class="middle tab-bar-section">
            <h1 class="title">Header Title</h1>
          </section>

          <section class="right-small">
            <a class="right-off-canvas-toggle menu-icon" ><span></span></a>
          </section>
        </nav>

        <aside class="left-off-canvas-menu">
          <ul class="off-canvas-list">
            <li><label>First Left Header</label></li>
            <li><a href="#">First Sub-Link</a></li>
          </ul>
        </aside>

        <aside class="right-off-canvas-menu">
          <ul class="off-canvas-list">
            <li><label>First Right Header</label></li>
            <li><a href="#">First Sub-Link</a></li>
          </ul>
        </aside>

        <section class="main-section">
          Main Content Here
        </section>

      <a class="exit-off-canvas"></a>

      </div>
    </div>

### `zf-top-bar` - create a top bar

    <nav class="top-bar" data-topbar>
      <ul class="title-area">
        <li class="name">
          <h1><a href="#">Site Name</a></h1>
        </li>
        <li class="toggle-topbar menu-icon"><a href="#">Menu</a></li>
      </ul>

      <section class="top-bar-section">
        <!-- Right Nav Section -->
        <ul class="right">
          <li class="active"><a href="#">Right Button Active</a></li>
          <li class="has-dropdown">
            <a href="#">Right Button with Dropdown</a>
            <ul class="dropdown">
              <li><a href="#">First link in dropdown</a></li>
            </ul>
          </li>
        </ul>

        <!-- Left Nav Section -->
        <ul class="left">
          <li><a href="#">Left Nav Button</a></li>
        </ul>
      </section>
    </nav>

### `zf-side-nav` - create a side navigation list

    <ul class="side-nav">
      <li class="active"><a href="#">Link 1</a></li>
      <li><a href="#">Link 2</a></li>
      <li><a href="#">Link 3</a></li>
      <li class="divider"></li>
      <li><a href="#">Link 4</a></li>
      <li><a href="#">Link 5</a></li>
    </ul>

### `zf-magellan` - create a magellan navigation list

    <div data-magellan-expedition="fixed">
      <dl class="sub-nav">
        <dd data-magellan-arrival="div1"><a href="#div1">Link 1</a></dd>
        <dd data-magellan-arrival="div2"><a href="#div2">Link 2</a></dd>
      </dl>
    </div>

### `zf-sub-nav` - create a sub-navigation list

    <dl class="sub-nav">
      <dt>Filter:</dt>
      <dd class="active"><a href="#">All</a></dd>
      <dd><a href="#">Active</a></dd>
      <dd><a href="#">Pending</a></dd>
      <dd><a href="#">Suspended</a></dd>
    </dl>

### `zf-breadcrumb` - create a breadcrumb block

    <nav class="breadcrumbs">
      <a href="#">Link 1</a>
      <a href="#">Link 2</a>
      <a class="unavailable" href="#">Link 3</a>
      <a class="current" href="#">Link 4</a>
    </nav>

### `zf-pagination` - create a pagination block

    <ul class="pagination">
      <li class="arrow unavailable"><a href="">&laquo;</a></li>
      <li class="current"><a href="">1</a></li>
      <li><a href="#">2</a></li>
      <li class="unavailable"><a href="">&hellip;</a></li>
      <li><a href="#">6</a></li>
      <li><a href="#">7</a></li>
      <li class="arrow"><a href="">&raquo;</a></li>
    </ul>

## Forms

### `zf-form` - create a form

    <form>
      <div class="row">
        <div class="large-2 columns">
          <label for="right-inline" class="right inline">Right Inline Label</label>
        </div>
        <div class="large-10 columns">
          <input type="text" id="right-inline" placeholder="large-9.columns" />
        </div>
      </div>
      <div class="row">
        <div class="large-4 columns">
          <label>Input Label
            <input type="text" placeholder="large-4.columns" />
          </label>
        </div>
        <div class="large-4 columns">
          <label>Input Label
            <input type="text" placeholder="large-4.columns" />
          </label>
        </div>
        <div class="large-4 columns">
          <div class="row collapse">
            <label for="postfix">Input Label</label>
            <div class="small-9 columns">
              <input type="text" id="postfix" placeholder="small-9.columns" />
            </div>
            <div class="small-3 columns">
              <span class="postfix">.com</span>
            </div>
          </div>
        </div>
      </div>
      <div class="row">
        <div class="large-12 columns">
          <label>Select Box
            <select>
              <option value="one">One</option>
              <option value="two">Two</option>
              <option value="three">Three</option>
              <option value="four">Four</option>
            </select>
          </label>
        </div>
      </div>
      <div class="row">
        <div class="large-6 columns">
          <label>Choose Your Favorite</label>
          <input type="radio" name="radio" value="true" id="true"><label for="true">True</label>
          <input type="radio" name="radio" value="false" id="false"><label for="false">False</label>
        </div>
        <div class="large-6 columns">
          <label>Check these out</label>
          <input id="checkbox1" type="checkbox"><label for="checkbox1">Checkbox 1</label>
          <input id="checkbox2" type="checkbox"><label for="checkbox2">Checkbox 2</label>
        </div>
      </div>
      <div class="row">
        <div class="large-12 columns">
          <label>Textarea Label
            <textarea placeholder="large-12.columns"></textarea>
          </label>
        </div>
      </div>
    </form>

### `zf-slider` - create a slider

    <div class="range-slider" data-slider data-options="[step:5; start:1; end:20; initial: 5]">
      <span class="range-slider-handle"></span>
      <span class="range-slider-active-segment"></span>
      <input type="hidden">
    </div>

## Media

### `zf-orbit` - create an orbit slider

    <ul class="example-orbit" data-orbit>
      <li>
        <img src="http://dummyimage.com/1000x400/4d494d/686a82.gif&text=Slide+1" alt="slide 1" />
        <div class="orbit-caption">
          Caption One.
        </div>
      </li>
      <li>
        <img src="http://dummyimage.com/1000x400/4d494d/68aa82.gif&text=Slide+2" alt="slide 2" />
        <div class="orbit-caption">
          Caption Two.
        </div>
      </li>
      <li>
        <img src="http://dummyimage.com/1000x400/4d494d/aa6a82.gif&text=Slide+3" alt="slide 3" />
        <div class="orbit-caption">
          Caption Three.
        </div>
      </li>
    </ul>

### `zf-thumb` - create a thumbnail

    <a class="th [radius]" href="http://dummyimage.com/1000x400/4d494d/686a82.gif&text=Large+Thumb">
      <img src="http://dummyimage.com/100x100/4d494d/686a82.gif&text=Thumb">
    </a>

### `zf-clearing` - create a clearing thumbnail list

    <ul class="clearing-thumbs" data-clearing>
      <li><a href="http://dummyimage.com/1000x400/4d494d/686a82.gif&text=Large Thumb"><img data-caption="Caption 1" src="http://dummyimage.com/100x100/4d494d/686a82.gif&text=Thumb"></a></li>
      <li><a href="http://dummyimage.com/1000x400/4d494d/68aa82.gif&text=Large Thumb"><img data-caption="Caption 2" src="http://dummyimage.com/100x100/4d494d/68aa82.gif&text=Thumb"></a></li>
      <li><a href="http://dummyimage.com/1000x400/4d494d/aa6a82.gif&text=Large Thumb"><img data-caption="Caption 3" src="http://dummyimage.com/100x100/4d494d/aa6a82.gif&text=Thumb"></a></li>
    </ul>

### `zf-flex-video` - create a flex video

    <div class="flex-video widescreen">
      <iframe width="500" height="250" src="Video Source" frameborder="0" allowfullscreen></iframe>
    </div>

### `zf-reveal` - create a flex video

    <a href="#" data-reveal-id="myModal" class="button">Modal Button</a>
    <div id="myModal" class="reveal-modal" data-reveal>
      <h2>This is the Heading</h2>
      <p class="lead">This is the lead</p>
      <p>This is the paragraph</p>
      <a class="close-reveal-modal">&#215;</a>
    </div>

## Credit
Inspiration from - https://github.com/zurb/foundation-5-sublime-snippets