# Gridify
A utility-first CSS Grid library. Inspired by larger open source libraries.

## Requirements
dart-sass

## Config
Create the following configuration variables (SCSS) before importing the grid CSS:
(Values below are just examples)
```
$grid-gap-base: 1rem;
$min-screen-size-sm: 300px;
$min-screen-size-md: 600px;
$min-screen-size-lg: 1000px;
$min-screen-size-xl: 1400px;

$max-gap-variants: 10;
$max-columns: 12;
$max-rows: 12;
```

## Usage
Simply import ```gridify.scss``` into your application's styling!


```
<h1>6 Column Grid (Responsive)</h1>

<section class="gfy-grid gfy-grid-gap:2 gfy-grid-cols:6">
  <div class="gfy-col-span:6 gfy-col-span:sm:4 gfy-col-span:md:3 gfy-col-span:lg:5 gfy-col-span:xl:2">1</div>
  <div class="gfy-col-span:3 gfy-col-span:sm:2 gfy-col-span:md:3 gfy-col-span:lg:1 gfy-col-span:xl:4">2</div>
  <div class="gfy-col-span:3 gfy-col-span:sm:2 gfy-col-span:md:3 gfy-col-span:lg:4 gfy-col-span:xl:2">3</div>
  <div class="gfy-col-span:6 gfy-col-span:sm:4 gfy-col-span:md:3 gfy-col-span:lg:2 gfy-col-span:xl:4">4</div>
</section>
```

All Gridify classes are prepended with ```gfy-``` to help prevent class name conflicts.