<template lang="pug">
  main
    section
      div.imgContainer
        nuxt-img(class="main__img",src="/image-header-desktop.jpg", alt="office")
      div.mainContainer  
        div.textContainer
          div.main__title
            h1.titulo Get 
              span insights 
              | that help your business grow.  
          p.main__paragraph Discover the benefits of data analytics and make better decisions regarding revenue, customer experience, and overall efficiency.
        div.articles
          article
            h1 10k+
            p COMPANIES
          article
            h1 314
            p TEMPLATES
          article
            h1 12M+
            p QUERIES
</template>
<style lang="scss" scoped>
@import '@/assets/styles/global.scss';
main {
  display: flex;
  justify-content: center;
  width: 100vw;
  height: 100vh;
  background: $Verydarkblue;
}
@media (min-width: 320px) {
  section {
    h1 {
      color: $White;
      font-family: $Inter;
      font-weight: 700;
    }
    span {
      font-weight: 700;
    }
    display: flex;
    flex-direction: column;
    align-items: center;
    background: $DarkDesaturated;
    width: 90%;
    max-height: 90%;
    margin: auto;
    border-radius: 5px;
    padding-bottom: 15px;
    .imgContainer {
      display: flex;
      width: 100%;
      height: fit-content;
      background-color: hsl(277, 88%, 35%);
      .main__img {
        width: 100%;
        border-radius: 5px 5px 0px 0px;
        opacity: 0.5;
      }
    }
    .textContainer{
      display: flex;
      flex-direction: column;
      align-items: center;
      .main__title {
        display: flex;
        justify-content: center;
        margin: 20px 0 15px 0;
        width: 85%;
        .titulo {
          text-align: center;
          width: 80%;
          span {
            color: $Softviolet;
          }
        }
      }
      .main__paragraph {
        color: $SlightlytransparentwhiteMAIN;
        text-align: center;
        width: 88%;
        line-height: 1.6;
      }
    }
    article {
      margin: 20px 0 20px 0;
      text-align: center;
      h1 {
        font-weight: 700;
      }
      p {
        margin-top: 6px;
        color: $Slightlytransparentwhite;
        font-size: 0.8em;
      }
    }
  }
}
@media (min-width: 1430px) {
  main{
    section {
      flex-direction: row;
      padding: 0;
      height: 55%;
      width: 75%;
      border-radius: 7px;
      .imgContainer{
        height: 100%;
        width: 50%;
        order: 4;
        border-radius: 0px 7px 7px 0px;
        overflow: hidden;
        .main__img {
          opacity: 0.5;
        }
      }
      .mainContainer{
        width: 50%;
        height: 75%;
        .textContainer{
          align-items: flex-start;
          margin-left: 70px;
          .main__title{
            justify-content: flex-start;
            .titulo{
              text-align: left;
              width: 105%;
              font-size: 2.5rem;
            }
          }
          .main__paragraph{
            text-align: left;
            width: 80%;
            margin: 15px 0px 55px 0px;
          }
        }
      }
    }
    .articles{
      align-self: flex-end;
      justify-self: flex-end;
      display: flex;
      flex-direction: row;
      justify-content: space-evenly;
      article{
        margin-right: 25px;
      }
    }
  }
}
</style>
