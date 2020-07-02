<template>
  <div>
    <div class="hero">
      <img src="~/assets/globe.jpg" class="hero-image">

      <div class="hero-imageOverlay">
        <div class="hero-message">
          海外アプローチを簡単に
        </div>
        <a href="#form" class="hero-contactButton">事前登録</a>
      </div>

    </div>

     <div class="strengthOverview">
      <div class="content">
        <!--<div class="headline">Abroarchの特徴</div>-->
        <div class="strength">
          <div class="strength-headline">
            <span class="strength-textBlock">
              <span class="strength-emph">海外ビジネス</span>に関する
            </span>
            <span class="strength-textBlock">
              <span class="strength-emph">初期的情報</span>
              を
            </span>
            <span class="strength-textBlock">
              <span class="strength-emph">安価</span>
              に取得可能
            </span>
          </div>
          <div class="strength-description">
            <p>
              現在、海外の一般的な情報は簡単にインターネットで取得することが出来ます。
            </p>
            <p>しかし、一歩踏み込んで業界プレイヤー・規制情報・投資環境等の情報を取得しようとした時にインターネットでは簡単に情報を取得することができません。</p>
            <p>また、専門の調査会社やコンサルタントに依頼をすると高額な費用がかかってしまい、海外ビジネス検討における初期的情報の収集には利用が難しいです。</p>
            <p>Abroachはそのような課題を解決すること目的としています。</p>
          </div>
        </div>
      </div>
    </div>

    <div class="serviceOverview">
      <div class="content">
        <div class="headline">Abroarchでできること</div>
        <p>様々なニーズに応じた海外ビジネス情報を取得することができます。</p>

        <div class="issueList">

          <div class="issue">
            <img class="issue-person" src="~/assets/person.png">
            <div class="speach">
              <div class="speach-bubble">開拓を検討中の海外市場で競合となるプレイヤーが知りたい</div>
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
              <div class="speach-bubble">海外市場に投入しようとしている商品に関する規制について知りたい</div>
            </div>
          </div>

           <div class="issue">
            <img class="issue-person" src="~/assets/person.png">
            <div class="speach">
              <div class="speach-bubble">海外企業の買収を検討しており、資本規制について知りたい</div>
            </div>
          </div>

        </div>

        <p></p>

      </div>
    </div>

    <div class="plans">
      <div class="content">
        <div class="headline">サービス形態</div>
        <p>お探しの情報に合わせて構築済みレポート、カスタム調査によるレポートをご選びいただけます。</p>
        <div class="plansWrapper">

          <div class="plan">
            <div class="plan-header">
              <img class="plan-image" src="~/assets/premade.png">
              <div class="plan-name">構築済みレポート</div>
            </div>
            <div class="plan-description">
              <ul>
                <li>基本統計情報</li>
                <li>規制情報</li>
                <li>投資環境</li>
                <li>業界概要</li>
                <li>業界プレイヤー等...</li>
              </ul>
            </div>
          </div>

          <div class="plan">
            <div class="plan-header">
              <img class="plan-image" src="~/assets/custommade.png">
              <div class="plan-name">カスタムレポート</div>
            </div>
            <div class="plan-description">
              <ul>
                <li>ご希望の海外ビジネス情報をカスタムレポートとしてご提供いたします。</li>
              </ul>
            </div>
          </div>

        </div>
      </div>
    </div>

    <div id="form" class="preRegisterForm">
      <div class="content">
        <div class="headline">事前登録</div>
        <p>現在当サービスは開発中です。以下よりご登録頂いた企業様にサービスの開発の状況等を共有いたします。</p>
        <div class="googleFormWrapper">
          <iframe class="googleForm" src="https://docs.google.com/forms/d/e/1FAIpQLSeryc4vFa8mBoSHSPb08ez39A3KlZES0tLsMBCtMiUREaa2gg/viewform?embedded=true" frameborder="0" marginheight="0" marginwidth="0">読み込んでいます…</iframe>
        </div>
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
  color: #555;
  font-size: 13pt;
  font-weight: 400;
}

.content {
  max-width: 1100px;
  padding: 0 20px;
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
  margin: 20px 0 10px 0;
  font-size: 23pt;
  font-weight: 700;
}

.issueList {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  justify-content: space-between;
  margin: 20px 10px;
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
    border-color: transparent $primaryDark transparent transparent;
    border-width: 10px 20px 10px 0;
  }

  &-bubble {
    padding: 10px;
    display: flex;
    align-items: center;
    max-width: 380px;
    height: 60px;
    border-radius: 10px;
    background: $primaryDark;
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
    max-width: 700px; 
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
    background: $primaryDark;
    border-radius: 30px;
    transition: background 0.2s;
  }

  &-contactButton:hover {
    background: $primary;
  }
}

.plansWrapper {
  width: 100%;
  height: 80%;
  display: flex;
  align-items: center;
  justify-content:space-around;
}

.plan {
  width: 300px;
  height: 330px;
  margin-top: 30px;
  display: flex;
  flex-direction: column;
  justify-content: start;
  align-items: center;
  background: white;
  border-radius: 10px;
  box-shadow: 1px 2px 5px #555;

  &-header {
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  &-image {
    width: 100px;
    height: 100px;
    margin: 20px 0 25px 0;
  }

  &-name {
    font-weight: 600;
    font-size: 17pt;
    color: $primaryDark;
    margin-bottom: 5px;
  }

  &-description {
    width: 80%;
    font-size: 11pt;
  }

  &-description li {
    list-style: '✔ ';
  }
}

.strength {
  margin-top: 15px;
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

  &-headline {
    font-size: 22pt;
    text-align: center;
  }

  &-emph {
    font-size: 28pt;
    font-weight: 700;
    color: $primaryDark;
  }

  &-textBlock {
    display: inline-block;
  }

  &-description {
    max-width: 650px;
    text-align: center;

    & p {
      font-size: 12pt;
      margin: 15px 0;
    }

  }
}

.googleFormWrapper {
  width: 100%;
  height: 1200px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.googleForm {
  width: 650px;
  height: 1050px;
}

.serviceOverview {
  background-color: #eee;
  height: 400px;
}

.plans {
  height: 550px;
}

.strengthOverview {
  height: 430px;
}

.preRegisterForm {
  background-color: #eee;
  height: 1300px;
}

@media(max-width: 1050px) {
.issue {
  &-person {
    width: 50px;
    height: 50px;
  }
}

.speach {
  &-bubble {
    max-width: 300px;
    height: 50px;
    border-radius: 5px;
    font-size: 10pt;
  }
}
}

@media(max-width: 860px) {
p {
  font-size: 10pt;
}

.hero {
  height: 300px;

  &-message {
    max-width: 340px; 
    font-size: 20pt;
  }

  &-contactButton {
    font-size: 11pt;
    font-weight: 500;
    padding: 8px 25px;
    border-radius: 30px;
  }

}

.headline {
  margin: 20px 0 10px 0;
  font-size: 16pt;
}

.sp-strength-headline {
  display: block;
}

.strengthOverview {
  height: 330px;
}

.strength {
  &-headline {
    font-size: 12pt;
  }

  &-emph {
    font-size: 17pt;
  }

  &-description {
    max-width: 500px;
    text-align: center;

    & p {
      font-size: 9pt;
    }
  }
}

.issueList {
  flex-direction: column;
  align-items: center;
}

.issue {
  margin: 7px 0;

  &-person {
    width: 35px;
    height: 35px;
  }
}

.speach {
  display: flex;
  align-items: center;

  &-bubble {
    height: 40px;
    border-radius: 5px;
    font-size: 9pt;
  }
}

.plansWrapper {
  flex-direction: column;
}

.plan {
  max-width: 400px;
  height: 160px;
  margin-top: 10px;

  &-header {
    flex-direction: row;
  }

  &-image {
    width: 25px;
    height: 25px;
    margin: 15px 10px;
  }

  &-name {
    font-size: 13pt;
  }

  &-description {
    font-size: 9pt;
  }

}

.googleFormWrapper {
  height: 1100px;
}

}

</style>
