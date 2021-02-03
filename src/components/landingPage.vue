<template>
  <div>
    <v-card class="mx-auto mt-10 mb-10" max-width="1165px" max-height="482px">
      <v-img class="white--text align-center" height="482px" src="@/assets/mie ayam.jpg">
        <v-card-title class="title">
          Cari tempat makan mie ayam
          <br />sekarang ga ribet lagi
        </v-card-title>
        <v-card-text class="sub-title mt-1">
          Berbagai tempat mie ayam yang enak akan ditunjukkan disini.
          <br />Temukan tempat yang cocok dengan seleramu.
        </v-card-text>
      </v-img>

      <!-- searc tombol -->

      <v-toolbar class="btn-toolbar" dense floating>
        <v-text-field placeholder="jelajahi disini.."></v-text-field>
        <v-btn color="#F15F31" id="searching" href="/recomendation">
          <p id="search">cari</p>
          <v-icon color="white">mdi-magnify</v-icon>
        </v-btn>
      </v-toolbar>
    </v-card>
    <!-- akhir search tombol -->

    <!-- content -->
    <v-container class="sub-container">
      <v-row class="mb-6" no-gutters>
        <v-col md="6" justify-center>
          <h2>REENPRESENT</h2>
          <br />
          <br />
          <p>
            REENPRESENTS memberikan informasi
            tentang tempat
            <br />makanan mie ayam
            yang ada di Yogyakarta,alamat tempat
            <br />makan,harga, dan ciri khasnya
          </p>
        </v-col>

        <v-col md="6">
          <v-card class="ml-10" max-width="300px">
            <v-img id="image" src="@/assets/logo mie.jpg" width="300px" height="300px"></v-img>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
    <v-container>
      <v-row class="hero">
        <v-col v-for="(barang,index) in barangs" :key="index" md="4">
          <v-row>
            <v-card>
              <v-card-title>
                <img :src="barang.gambar" />
                <v-card-actions>
                  {{barang.nama}}
                  <v-list-item>{{barang.harga}}</v-list-item>
                </v-card-actions>
                <!-- <v-card-text>{{barang.harga}}</v-card-text> -->
                <v-spacer></v-spacer>
                <v-card>
                  {{barang.jalan}}
                  <v-spacer></v-spacer>
                  <v-list-item>{{barang.rating}}</v-list-item>
                </v-card>
              </v-card-title>
            </v-card>
          </v-row>
        </v-col>
      </v-row>
    </v-container>
    <!-- Akhir content -->
  </div>
</template>
<script>
export default {
  components: {},
  data: () => {
    return {
      barangs: [
        {
          nama: "Tumini Asri",
          jalan: "jl paris",
          harga: 10000,
          rating: "4,5",
          gambar: "/assets/logo.png"
        },
        {
          nama: "Tumini Asri",
          jalan: "jl paris",
          harga: 10000,
          rating: "4,5",
          gambar: "/assets/logo.png"
        },
        {
          nama: "Tumini Asri",
          jalan: "jl paris",
          harga: 10000,
          rating: "4,5",
          gambar: "/assets/logo.png"
        },

        {
          nama: "Tumini Asri",
          jalan: "jl paris",
          harga: 10000,
          rating: "4,5",
          gambar: "/assets/logo.png"
        },
        {
          nama: "Tumini Asri",
          jalan: "jl paris",
          harga: 10000,
          rating: "4,5",
          gambar: "/assets/logo.png"
        },
        {
          nama: "Tumini Asri",
          jalan: "jl paris",
          harga: 10000,
          rating: "4,5",
          gambar: "/assets/logo.png"
        }
      ]
    };
  }
};
</script>




<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@100;400&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@100;400&family=Roboto&display=swap");

.title {
  font-family: "Poppins", sans-serif !important;
  font-size: 28px !important;
}
.sub-title {
  font-family: "Poppins", sans-serif !important;
  font-size: 18px !important;
}
.btn-toolbar {
  margin-left: 20px;
  margin-top: -30px;
  width: 500px;
  box-shadow: 2px 2px 2px rgba(0, 0, 0, 0) !important;
}

.sub-container {
  margin-top: 300px;
  margin-left: 100px;
}
p {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
#image {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-bottom: 600px;
  margin-top: -100px;
}
#search {
  color: white !important;
  margin: 13px 5px;
  width: 50px;
}
#searching {
  margin-left: 300px;
  width: 100px;
}

.hero {
  margin-top: -400px;
  margin-right: 10px;
  padding: 10px;
}
h2 {
  margin-left: 160px;
  margin-top: -70px;
}
</style>