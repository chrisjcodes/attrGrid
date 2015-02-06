# attrGrid
A configureable LESS grid that uses data attributes rather than classes and is based on fixed widths

*I essentially built this for my own usage because Im particular. There are far too many grids in the world*

## Usage
In your *style.less* file import the grid as so
```
@import "attrgrid";
```

### Setting Up Grid
Open up *attrgrid.less* and set the following to your preferences
```
@maxGrid: 1080px;
@tabletMax: 959px;
@mobileMax: 768px;
@columns:16;
@gutter: 10px;
```

### Markup
After that youre ready to go. Each time you use the grid you must wrap it in a data-container, like so
```
<div data-container>
<!--Grid all up in here-->
</div>
```

The number of columns you have available depends on what you set but an example of setting the columns would look like this
```
<div data-columns="4">
<!--content all up in here-->
</div>
```

### Constants
**Clear** is available but the grid is self clearing so its not needed

**Full** is an option that lets you set an element to the max width of your grid *Note: this is not the full page width*
```
<div data-columns="full">
<!--I span the max number of columns-->
</div>
```

You can also use **3rds**
```
<div data-columns="1-3">
<!--I'm 1/3-->
</div>

<div data-columns="2-3">
<!--I'm 2/3-->
</div>
```

Attr do grid, attr do.

