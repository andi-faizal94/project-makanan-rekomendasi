<template>
  <div>
    <v-card v-for="(barang,index) in barangs" :key="index">
      {{barang.nama}},
      <img :src="barang.gambar" />
    </v-card>
  </div>
</template>

<script>
export default {
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
          nama: "Tunggal Rasa Kota Baru",
          jalan: "jl paris",
          harga: 10000,
          rating: "4,5",
          gambar: ""
        },
        {
          nama: "Palembang Afui",
          jalan: "jl paris",
          harga: 10000,
          rating: "4,5",
          gambar: ""
        },
        {
          nama: "Jogja",
          jalan: "jl paris",
          harga: 10000,
          rating: "4,5",
          gambar: ""
        },
        {
          nama: "Bandung 59",
          jalan: "jl paris",
          harga: 10000,
          rating: "4,5",
          gambar: ""
        },

        {
          nama: "Pak Wadi",
          jalan: "jl paris",
          harga: 10000,
          rating: "4,5",
          gambar: ""
        },
        {
          nama: "Kameha Timoho",
          jalan: "jl paris",
          harga: 10000,
          rating: "4,5",
          gambar: ""
        },
        {
          nama: "Jakarta",
          jalan: "jl paris",
          harga: 10000,
          rating: "4,5",
          gambar: ""
        },
        {
          nama: "Jakarta",
          jalan: "jl paris",
          harga: 10000,
          rating: "4,5",
          gambar: ""
        },
        {
          nama: "Jakarta",
          jalan: "jl paris",
          harga: 10000,
          rating: "4,5",
          gambar: ""
        },
        {
          nama: "Jakarta",
          jalan: "jl paris",
          harga: 10000,
          rating: "4,5",
          gambar: ""
        },
        {
          nama: "Jakarta",
          jalan: "jl paris",
          harga: 10000,
          rating: "4,5",
          gambar: ""
        },
        {
          nama: "Jakarta",
          jalan: "jl paris",
          harga: 10000,
          rating: "4,5",
          gambar: ""
        },
        {
          nama: "Jakarta",
          jalan: "jl paris",
          harga: 10000,
          rating: "4,5",
          gambar: ""
        },
        {
          nama: "Jakarta",
          jalan: "jl paris",
          harga: 10000,
          rating: "4,5",
          gambar: ""
        }
      ]
    };
  }
};
</script>

<style>
</style>