<template>
<!--mainの最初の奴です。-->
  <div class="template">
    <div class="mainleft">
      <MainLeft/> 
    </div>
    <table class="table">
      <th class="th-option1">ホーム</th>
      <tr>
        <td>test</td>
        <td><img height="13px" width="13px" src="../assets/img/heart.png" alt=""></td>
        <td><img height="13px" width="13px" src="../assets/img/cross.png" alt=""></td>
        <NuxtLink to="/comment"><td><img height="13px" width="13px" src="../assets/img/detail.png" alt=""></td></NuxtLink>
      </tr>
    </table>
  </div>
</template>

<script>
export default {}
</script>

