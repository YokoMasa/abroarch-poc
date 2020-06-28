<template>
  <div>
    <div class="hero">
      <img src="~/assets/globe.jpg" class="hero-image">

      <div class="hero-imageOverlay">
        <div class="hero-message">
          キャッチコピー
        </div>
        <a href="#form" class="hero-contactButton">事前登録</a>
      </div>

    </div>

    <div class="serviceOverview">
      <div class="content">
        <div class="headline">Abroarchでできること</div>
        <p>様々なニーズに応じた海外ビジネス情報を得ることができます。</p>

        <div class="issueList">

          <div class="issue">
            <img class="issue-person" src="~/assets/person.png">
            <div class="speach">
              <div class="speach-bubble">開拓を検討中の海外市場に関する情報が欲しい</div>
            </div>
          </div>

           <div class="issue">
            <img class="issue-person" src="~/assets/person.png">
            <div class="speach">
              <div class="speach-bubble">海外人材活用の検討に当たって海外の労働事情・関係法を知りたい</div>
            </div>
          </div>

           <div class="issue">
            <img class="issue-person" src="~/assets/person.png">
            <div class="speach">
              <div class="speach-bubble">xxx</div>
            </div>
          </div>

           <div class="issue">
            <img class="issue-person" src="~/assets/person.png">
            <div class="speach">
              <div class="speach-bubble">xxx</div>
            </div>
          </div>

        </div>

        <p></p>

      </div>
    </div>

    <div class="plans" style="background: #eee">
      <div class="content">
        <div class="headline">サービス形態</div>
        <p>xxx</p>
        <div class="plansWrapper">
          <div class="plan">
            <p class="plan-name">構築済みレポートの提供</p>
          </div>
          <div class="plan">
            <p class="plan-name">カスタムレポートの提供</p>
          </div>
        </div>
      </div>
    </div>

    <div class="serviceOverview">
      <div class="content">
        <div class="headline">Abroarchの特徴（既存ソリューションには無い強み）</div>
      </div>
    </div>

    <div id="form" class="serviceOverview" style="background: #eee">
      <div class="content">
        <div class="headline">事前登録フォーム</div>
        <p>google formsでメールアドレス入力？</p>
      </div>
    </div>

    <div class="serviceOverview">
      <div class="content">
        <div class="headline">Creww協賛について</div>
        <p>不要？</p>
      </div>
    </div>

  </div>
</template>

<script>
export default {
 
}
</script>

<style scoped lang="scss">
$primary: #2195f2;
$primaryLight: #6ec5ff;
$primaryDark: #0068bf;

p {
  font-size: 15pt;
  font-weight: 600;
}

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

.headline {
  display: inline-block;
  margin: 20px 0;
  font-size: 20pt;
  font-weight: 700;
  border-bottom: solid 3px #555 ;
}

.issueList {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  justify-content: space-between;
  margin: 30px;
}

.issue {
  display: flex;
  align-items: center;
  margin: 20px 0;

  &-person {
    width: 60px;
    height: 60px;
  }
}

.speach {
  display: flex;
  align-items: center;

  &:before {
    content: "";
    width: 0px;
    height: 0px;
    border-style: solid;
    border-color: transparent $primary transparent transparent;
    border-width: 10px 20px 10px 0;
  }

  &-bubble {
    padding: 10px;
    display: flex;
    align-items: center;
    width: 380px;
    height: 60px;
    border-radius: 10px;
    background: $primary;
    color: white;
  }
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

.plansWrapper {
  width: 100%;
  height: 80%;
  display: flex;
  align-items: center;
  justify-content: space-evenly;
}

.plan {
  width: 300px;
  height: 300px;
  background: $primary;
  border-radius: 30px;

  &-name {
    font-size: 14pt;
    text-align: center;
    color: white;
    border-bottom: 2px solid white;
  }

}

.serviceOverview {
  height: 400px;
}

.plans {
  height: 500px;
}


</style>
