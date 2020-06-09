<template>
  <div>
    <div class="hero">
      <img src="~/assets/globe.jpg" class="hero-image">

      <div class="hero-imageOverlay">
        <div class="hero-message">
          訴求メッセージ
        </div>
        <a href="#form" class="hero-contactButton">事前登録</a>
      </div>

    </div>

    <div class="serviceOverview">
      <div class="content">
        <h1>こんな課題ありませんか？</h1>
      </div>
    </div>

    <div class="serviceOverview" style="background: #ddd">
      <div class="content">
        <h1>このサービスで何ができるの？</h1>
      </div>
    </div>

    <div class="serviceOverview">
      <div class="content">
        <h1>サービス詳細</h1>
      </div>
    </div>

    <div id="form" class="serviceOverview" style="background: #ddd">
      <div class="content">
        <h1>事前登録フォーム</h1>
        google formsでメールアドレス入力？
      </div>
    </div>
  </div>
</template>

<script>
export default {
 
}
</script>

<style lang="scss">
$primary: #2195f2;
$primaryLight: #6ec5ff;
$primaryDark: #0068bf;

.content {
  max-width: 1100px;
  height: 100%;
  margin-left: auto;
  margin-right: auto;
}

.flex-center {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.hero {
  position: relative;
  width: 100%;
  height: 600px;

  &-image {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }

  &-imageOverlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(white, 0.7);
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }

  &-message {
    word-break: break-all;
    max-width:400px; 
    font-size: 35pt;
    font-weight: 600;
    margin-bottom: 30px;
  }

  &-contactButton {
    text-decoration: none;
    color: white;
    font-size: 14pt;
    font-weight: 600;
    padding: 10px 50px;
    background: $primary;
    border-radius: 30px;
    transition: background 0.2s;
  }

  &-contactButton:hover {
    background: $primaryLight;
  }
}

.serviceOverview {
  height: 600px;
}
</style>
