---
layout: post
title:  Free Code Camp Note
date:   2019-01-31 10:05
categories: code_collection
tags: css
---

* content
{: toc}


### margin:0 auto can be used to center things
the 0 is bottom and top, and `auto` is auto setting the left and right.
just to resize the element you want to center, then use this `margin` setup,
without needing to use flex box.


### use !important to hack fontawesome size when using React fontawesome library
I tried to reset the size of the icons with the `div` wrapper, it didn't work.
however, I can hack this by using the `!important`, since it's only changing the size of
the icons, it won't mess things up in the future.

```css
.social_icon{


  width:30px !important;
  height:30px;
  color:white;
  margin-left:16px;
  margin-right:0;
  border-radius:100%;  
  text-align:right;  
  list-style:none;
}
```
### box-shadow for thumbnail

```css
#thumbnail{
  box-shadow: 0 10px 20px rgba(0,0,0,0.19), 0 6px 6px rgba(0,0,0,0.23);
}
```

### relative and absolute
https://jsbin.com/kenikuqulu/1/edit?css,js,output

### flex box workshop example
[flex box workshop](https://bit.ly/tjsworkshops)


### Gradual CSS Linear Gradient

```html
<style>
div{
  border-radious:20px;
  width:70%;
  height:400px;
  margin:50px auto;
  background:linear-gradient(35deg,#CCFFFF,#FFCCCC);
}
</style>

<div></div>
```
### Create stripes with `repeating-linear-gradient()`

```
  div{
    border-radius: 20px;
    width: 70%;
    height: 400px;
    margin:  50 auto;
    background: repeating-linear-gradient(
      45deg,
      yellow 0px,
      yellow 40px,
      black 40px,
      black 80px
    );
  }

</style>
```
### overflow-wrap
[checkout t](https://codepen.io/impressivewebs/pen/ZLBvav)

### grid model

[grid model](https://repl.it/@thinkful/CSS-Responsive-Grid-Challenge-Solution)


### Input with search icon
```
#search-input {
  background-image: url('https://www.w3schools.com/css/searchicon.png');
  background-position: 10px 12px;
  background-repeat: no-repeat;
  width: 100%;
  font-size: 16px;
  padding: 12px 20px 12px 40px;
  border: 1px solid #ddd;
  margin-bottom: 12px;
  margin-top:12px;
}
```

## React
### Message Notification
![img](https://tf-curricula-prod.s3.amazonaws.com/curricula/da13a510-00f5-4649-9416-c29d8f2f4761/ei-react-v1/assets2/react_testing_components/react_testing_06.png)
```
.messages{
  display:block;
  position:relative;
  padding: 0 12px;
  height:22px;
  line-height:26px;
  font-size:11px;
  font-weight:bold;
  color:#666;
  text-decoration: none;
  text-shadow: 0 1px white;
  background:#FAFAFA;
  width:100px;
  box-shadow:inset 0 0 3px rgba(0,0,0,0.1);
  margin:15px auto;

}

.messages .unread_count{
  display:block;
  position: absolute;
  top:-10px;
  right:3px;
  line-height:14px;
  height:14px;
  padding: 0 5px;
  font-family:Arial, sans-serif;
  font-size:9px;
  color:white;
  text-shadow:0 1px rgba(0,0,0,0.25);
  border:1px solid;
  border-radius:10px;
  box-shadow:inset 0 1px rgba(255,255,255,0.3),0 1px 1px;
  background:#67c1ef;
  border-color:#30aae9;
}


```

### put a div tag on top of everything with z index
```
 z-index: 99 !important;
```