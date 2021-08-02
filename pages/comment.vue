<template>
<!--mainの二つ目の奴です。-->
  <div class="template">

    <div class="mainleft">
      <MainLeft/>      
    </div>

    <table class="table">
      <th class="th-option1">コメント</th>
      <tr>
        <td>test</td>
        <td><img height="13px" width="13px" src="../assets/img/heart.png" alt=""></td>
        <td><img height="13px" width="13px" src="../assets/img/cross.png" alt=""></td>
      </tr>
      <th class="th-option2">コメント</th>
      <tr>
        <td>text</td>
      </tr>
    </table>

    <div class="comment-bottom">
      <validation-provider v-slot="ProviderProps" rules="required|max:120">
        <input v-model="name" name="コメント" type="text">
        <div class="error">{{ ProviderProps.errors[0] }}</div>
        <div class="error">{{ ProviderProps.errors[3] }}</div>        
      </validation-provider>
      <button>コメント</button>
    </div>
    
  </div>
</template>

<script>
export default {}
</script>

<style>
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

   
  a{
    text-decoration: none;
  }

  .template{
    background-color: rgb(25, 25, 37);
    height: 100vh;
    color: white;
    padding: 5px 0 0 10px;
  }
  .mainleft{
    float: left;
    margin-right: 50px;
  }

  .icon1{
  display:flex;
  margin-bottom: 10px;
  margin-top: 15px;
}
.icon1 p{
  padding-left: 10px;
  font-size: 13px;
  color: white;
}
.icon2{
  display: flex;
}
.icon2 p{
  padding-left: 10px;
  font-size: 13px;
  margin-bottom: 20px;
  color: white;
}


.share p{
  font-size: 13px;
  margin-bottom: 10px;
}

.textarea{
  background-color: rgb(25, 25, 37);
  border-radius: 10px;
}

.share button{
  position: absolute;
  top: 270px;
  left: 150px;
  background-color:rgb(65, 22, 184) ;
  border-radius: 100px;
  border: 1px solid rgb(65, 22, 184);
  font-size: 11px;
  height: 30px;
  width: 80px;
  color: white;
}

.th-option1{
  border-left: 1px solid white;
  border-bottom: 1px solid white;
  height: 10px;
  padding: 10px;
  width: 100vw;
  text-align: left;
}

.table td{
  width: 10px;
  display: inline-block;
  padding: 10px 15px;
}

.table tr{
  border-left: 1px solid white;
  border-bottom: 1px solid white;
}

.table button{
  text-align: left;
}

.th-option2{
  font-size: 12px;
  text-align: center;
  border-left: 1px solid white;
  border-bottom: 1px solid white;
  height: 10px;
  padding: 10px;
  width: 100vw;
}

.comment-bottom{
  text-align: center;
  margin-top: 20px;
}

.comment-bottom input{
  background-color: rgb(25, 25, 37);
  width: 750px;
  border-radius: 5px;
  border: 1px solid white;
  color: white;
}

.comment-bottom button{
  background-color:rgb(65, 22, 184) ;
  border-radius: 100px;
  border: 1px solid rgb(65, 22, 184);
  font-size: 11px;
  height: 30px;
  width: 80px;
  color: white;
  margin-top: 20px;
  margin-left: 700px;
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
