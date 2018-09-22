### CSS Grid options
- A basic starter project layouts on CSS Grids for webapps and SPAs/

### 1. News Layout
> This code below is for a HuffPost news type layout done via CSS Grids.

```css
/* Mobile first by default */

html {
  box-sizing: border-box;
}
*,
*:before,
*:after {
  box-sizing: inherit;
}
body {
  margin: 0px;
  padding: 0px;
}

/* Smartphones (portrait and landscape) ----------- */
@media only screen and (min-device-width: 320px) and (max-device-width: 480px) {
  /* Our  Main Container */
  .container {
    height: auto;
    display: grid;
  }

  /* Navbar */
  .navbar {
    grid-row: 1 / 2;
    grid-column: 1 / -1;
    height: auto;
    background-color: black;
  }
  /* ------------------------------ */
  /* Main Section */
  .main-content-wrapper {
    grid-row: 2 / 8;
    grid-column: 1 / -1;
    /* Styling */
    background-size: cover;
    background-position: 50% 50%;
    width: 100%;
  }
  /* ------------------------------ */
  /* Section One - Left */
  .sec-1-left {
    grid-row: 8 / 14;
    grid-column: 1 / -1;
  }

  /* Section Two - Center */
  .sec-2-center {
    grid-row: 14 / 16;
    grid-column: 1 / -1;
  }

  /* Section Three - Right */
  .sec-3-right {
    grid-row: 16 / 18;
    grid-column: 1 / -1;
  }
  .sec-4-right {
    grid-row: 18 / 21;
    grid-column: 1 / -1;
  }

  /* News Section */
  /* News Big Story */
  .news-big {
    grid-row: 21 / 23;
    grid-column: 1 / -1;
  }
  /* News story left */
  .news-left {
    grid-row: 23 / 25;
    grid-column: 1 / -1;
  }
  /* News story right */
  .news-right {
    grid-row: 25 / 27;
    grid-column: 1 / -1;
  }

  /* Trending Stories Section */
  .trending-stories {
    grid-row: 27 / 29;
    grid-column: 1 / -1;
  }
}

/* Small devices (tablets, 768px and up) */
@media (min-width: 550px) {
}

/* Desktops and laptops ----------- */
@media only screen and (min-width: 1224px) {
  /* Our  Main Container */
  .container {
    height: auto;
    display: grid;
    grid-gap: 0;
    grid-template-columns: repeat(auto-fit, minmax(100px, 1fr));
    grid-auto-rows: 25%;
    grid-auto-flow: dense;
  }
  /* ------------------------------- */
  /* Navbar */
  .navbar {
    grid-row: 1 / 2;
    grid-column: 1 / -1;
    /* height: 78px; */
    /* Navbar styling */
    height: auto;
    background-color: black;
    width: 100%;
    /* position: fixed; */
    top: 0;
    margin-bottom: 0;
  }
  /* ------------------------------- */
  /* Main Section */
  /* Main Section background Image*/
  .main-content-wrapper {
    grid-row: 2 / 8;
    grid-column: 1 / -1;
    /* height: 480px; */
    /* Styling */
    background-size: cover;
    background-position: 50% 50%;
    height: 480px;
  }
  /* ------------------------------- */
  /* Section One - Left */
  .sec-1-left {
    grid-row: 8 / 14;
    grid-column: 2 / 5;
    /* height: 680px; */
  }

  /* Section Two - Center */
  .sec-2-center {
    grid-row: 8 / 15;
    grid-column: 5 / 10;
    height: 850px;
  }

  /* Section Three - Right */
  .sec-3-right {
    grid-row: 8 / 13;
    grid-column: 10 / 13;
    /* height: 550px; */
  }
  .sec-4-right {
    grid-row: 13 / 16;
    grid-column: 10 / 13;
  }

  /* News Section */
  /* News Big Story */
  .news-big {
    grid-row: 16 / 19;
    grid-column: 2 / 10;
  }
  /* News story left */
  .news-left {
    grid-row: 19 / 21;
    grid-column: 2 / 6;
  }
  /* News story right */
  .news-right {
    grid-row: 19 / 21;
    grid-column: 6 / 10;
  }

  /* Trending Stories Section */
  .trending-stories {
    grid-row: 16 / 21;
    grid-column: 10 / 13;
  }
}
```
