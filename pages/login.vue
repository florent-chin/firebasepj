<template>
<!--ログイン画面です。-->
  <div class="template">
    
    <Header/>

    <div class="card">
      <p>ログイン</p>
      <validation-provider v-slot="ProviderProps" rules="required">
        <input v-model="name" name="メールアドレス" size="25" type="text" placeholder="メールアドレス">
        <div class="error">{{ ProviderProps.errors[0] }}</div>
      </validation-provider>  
      <validation-provider v-slot="ProviderProps" rules="required">
        <input v-model="name" name="パスワード" size="25" type="text" placeholder="パスワード">
        <div class="error">{{ ProviderProps.errors[0] }}</div>
      </validation-provider> 
      <NuxtLink to="/main">ログイン</NuxtLink>
    </div>

  </div>
</template>

