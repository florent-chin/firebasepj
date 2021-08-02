<template>
<!-- ヘッダー完全版です。 -->
  <div class="header">
    <div class="HeaderLogo">
      <HeaderLogo></HeaderLogo>
    </div>

    <div class="header-right">
      <NuxtLink to="/">新規登録</NuxtLink>
      <NuxtLink to="/login">ログイン</NuxtLink>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style>

  a{
    text-decoration: none;
  }

  .template{
    background-color: rgb(25, 25, 37);
    height: 100vh;
  }

  .header{
    height: 120px;
  }

  .HeaderLogo{
    float: left;
    margin: 10px;
  }

  .header-right{
    float: right;
    display: flex;
    margin: 20px;
  }
  .header-right a{
    margin-left: 20px;
    color: white;
  }

  .card{
    flex-direction: column;
    text-align: center;
    background-color: white;
    margin: 0 430px;
    padding: 20px 0;
    border-radius: 3px;
    width: 280px;
  }
  .card p{
    font-size: 14px;
    font-weight: bold;
  }
  .card input{
    display: block;
    margin: 10px auto;
    border-radius: 5px;
    border: 1px solid rgb(118, 118, 118);
    padding: 5px ;
    color: rgb(118, 118, 118);
  }
  .card a{
    display: block;
    margin: 0 100px;
    font-size: 10px;
    font-weight: bold;
    border-radius: 100px;
    border: 1px solid rgb(65, 22, 184);
    background-color: rgb(65, 22, 184);
    color: white;
    padding: 10px;
  }













  html, body, div, span, object, iframe,
h1, h2, h3, h4, h5, h6, p, blockquote, pre,
abbr, address, cite, code,
del, dfn, em, img, ins, kbd, q, samp,
small, strong, sub, sup, var,
b, i,
dl, dt, dd, ol, ul, li,
fieldset, form, label, legend,
table, caption, tbody, tfoot, thead, tr, th, td,
article, aside, canvas, details, figcaption, figure,
footer, header, hgroup, menu, nav, section, summary,
time, mark, audio, video {
    margin:0;
    padding:0;
    border:0;
    outline:0;
    font-size:100%;
    vertical-align:baseline;
    background:transparent;
}

body {
    line-height:1;
}

article,aside,details,figcaption,figure,
footer,header,hgroup,menu,nav,section {
    display:block;
}

nav ul {
    list-style:none;
}

blockquote, q {
    quotes:none;
}

blockquote:before, blockquote:after,
q:before, q:after {
    content:'';
    content:none;
}

a {
    margin:0;
    padding:0;
    font-size:100%;
    vertical-align:baseline;
    background:transparent;
}

/* change colours to suit your needs */
ins {
    background-color:#ff9;
    color:#000;
    text-decoration:none;
}

/* change colours to suit your needs */
mark {
    background-color:#ff9;
    color:#000;
    font-style:italic;
    font-weight:bold;
}

del {
    text-decoration: line-through;
}

abbr[title], dfn[title] {
    border-bottom:1px dotted;
    cursor:help;
}

table {
    border-collapse:collapse;
    border-spacing:0;
}

/* change border colour to suit your needs */
hr {
    display:block;
    height:1px;
    border:0;  
    border-top:1px solid #cccccc;
    margin:1em 0;
    padding:0;
}

input, select {
    vertical-align:middle;
}

</style>