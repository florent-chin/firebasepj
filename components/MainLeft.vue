<template>
<!-- 中身の左側の奴です。 -->
  <div>
    <HeaderLogo/> 

    <div class="icon1">
      <i class="fas fa-home"></i>
      <NuxtLink to="/main"><p>ホーム</p></NuxtLink>
    </div>
    <div class="icon2">
      <i class="fas fa-sign-out-alt"></i>
      <NuxtLink to="/login"><p>ログアウト</p></NuxtLink>
    </div>

    <div class="share">
      <p>シェア</p>
      <validation-provider v-slot="ProviderProps" rules="required|max:120">
        <textarea v-model="name" name="シェア" class="textarea" cols="28" rows="8"></textarea>
        <div class="error">{{ ProviderProps.errors[0] }}</div>
        <div class="error">{{ ProviderProps.errors[3] }}</div>
      </validation-provider>
      <br>
      <button>シェアする</button>
    </div>
  </div>
</template>

