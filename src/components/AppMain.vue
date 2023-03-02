<script>
import AppCard from './AppCard.vue'
export default {
  components: {
    AppCard
  },
  data() {
    return {
      comics: [
        {
          "thumb": "https://2.bp.blogspot.com/M3X0hC5MMVJ-5ZYFVPzfDxr_ytM1_voZTWUlKKF20EWC_bwQwYaxByNxgaY5x2e5OUQpgr9Ww0sf=s0?rhlupa=MjcuNjcuMTg1Ljc5&rnvuka=TW96aWxsYS81LjAgKExpbnV4OyBBbmRyb2lkIDYuMC4xOyBTTS1BNTIwRiBCdWlsZC9NTUIyOUspIEFwcGxlV2ViS2l0LzUzNy4zNiAoS0hUTUwsIGxpa2UgR2Vja28pIENocm9tZS82MC4wLjMxMTIuMTE2IE1vYmlsZSBTYWZhcmkvNTM3LjM2",
          "price": "$19.99",
          "series": "Action Comics",
          "type": "comic book"
        },
        {
          "thumb": "https://2.bp.blogspot.com/goluVzEqWfV_oBGXSXTmzqcu4jFsq_Uaq1lA1Gp4qaaaAc5Rd3NWfFX5T2riSU8H81WqqbGOa8nXfMU5byXi4Bxb7zGwEiDFTSqZhOhGPLDt8NFchjbzwlHroBEANdHdIZkaebpX=s0?rhlupa=MjcuNjcuMzIuMTQx&rnvuka=TW96aWxsYS81LjAgKExpbnV4OyBBbmRyb2lkIDQuNC4yOyBTTS1OOTAwUCBCdWlsZC9LT1Q0OUgpIEFwcGxlV2ViS2l0LzUzNy4zNiAoS0hUTUwsIGxpa2UgR2Vja28pIENocm9tZS82MC4wLjMxMTIuMTE2IE1vYmlsZSBTYWZhcmkvNTM3LjM2",
          "price": "$3.99",
          "series": "American Vampire 1976",
          "type": "comic book"
        },
        {
          "thumb": "https://i.pinimg.com/originals/32/dc/2b/32dc2b38c83c6faf58317851fe0bbc5c.jpg",
          "price": "$16.99",
          "series": "Aquaman",
          "type": "graphic novel"
        },
        {
          "thumb": "https://i.pinimg.com/originals/f7/b1/53/f7b153bd3e2fdfa70680525dc878945d.jpg",
          "price": "$2.99",
          "series": "Batgirl",
          "type": "comic book"
        },
        {
          "thumb": "https://static.dc.com/dc/files/default_images/BMULv4%2520%2528Cover%2529_63be1a7cebc624.37541381.jpg",
          "price": "$3.99",
          "series": "Batman",
          "type": "comic book"
        },
        {
          "thumb": "https://3.bp.blogspot.com/-Zz0pJuWICbY/VFI5M8Z_TFI/AAAAAAAFj3Q/89MY1NN1T70/s1600/p4_0%2Bcopy.jpg",
          "price": "$2.99",
          "series": "Batman Beyond",
          "type": "comic book"
        },
        {
          "thumb": "https://3.bp.blogspot.com/--bjxVyUbYzk/VaJ5Pt6GntI/AAAAAAANI2k/3GkraNSn-zk/s1600/p_34_00.jpg",
          "price": "$3.99",
          "series": "Batman/Superman",
          "type": "comic book"
        },
        {
          "thumb": "https://www.panini.co.uk/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/g/b/gbhtp005_0.jpg",
          "price": "$4.99",
          "series": "Batman/Superman Annual",
          "type": "comic book"
        },
        {
          "thumb": "https://www.ibs.it/images/9781406254099_0_424_0_75.jpg",
          "price": "$5.99",
          "series": "Batman: The Joker War Zone",
          "type": "comic book"
        },
        {
          "thumb": "https://m.media-amazon.com/images/I/51ikkHxJOqL._SX323_BO1,204,203,200_.jpg",
          "price": "$6.99",
          "series": "Batman: Three Jokers",
          "type": "comic book"
        },
        {
          "thumb": "https://static.dc.com/dc/files/default_images/BMULv4%2520%2528Cover%2529_63be1a7cebc624.37541381.jpg",
          "price": "$4.99",
          "series": "Batman: White Knight Presents: Harley Quinn",
          "type": "comic book"
        },
        {
          "thumb": "https://midulstergranite.com/images/images/i.gr-assets.com_images_S_compressed.photo.goodreads.com_books_1647384539l_60625998.jpg",
          "price": "$16.99",
          "series": "Catwoman",
          "type": "graphic novel"
        }
      ],
    }
  }
}

</script>

<template>
  <section class="jumbotron">
    <span class="tag font">
      CURRENT SERIES
    </span>
  </section>
  <section class="main">
    <div class="container">
      <ul class="row series">
        <AppCard class="col_series" v-for="(comic, i) in comics" :key="i" :series="comic.series" :thumb="comic.thumb">
        </AppCard>
      </ul>
    </div>
    <div class="more">
      <a href="#">
        <p class="font">LOAD MORE</p>
      </a>
    </div>
  </section>
</template>

<style lang="scss" scoped>
@use '../style/partials/variable' as *;
@use '../style/general.scss' as *;

.jumbotron {
  background-image: url('/img/jumbotron.jpg');
  background-position: top center;
  min-height: 400px;
  position: relative;
}

.tag {
  color: white;
  background-color: $color-active-link;
  padding: 15px;
  position: absolute;
  top: 95%;
  left: 21%;
  font-size: 18px;

}

.series {
  flex-wrap: wrap;
}

.col_series {
  flex-basis: calc(100%*(2/12));
}

.more {
  width: 200px;
  text-align: center;
  margin: 20px auto 0px auto;
  background-color: $color-active-link;
  color: white;
  padding: 10px 0px;
}

.main {
  padding: 40px 0px;
  background-color: #1C1C1C;
}

.content {
  color: white;
}
</style>