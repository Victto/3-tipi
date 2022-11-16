<template>
  <div class="divperfil" v-for="perfil in perfils">
    <img :src="perfil.fotoUrl" class="imgperfil" />
  </div>

  <h3>Mais Vendidos ></h3>
  <div class="divprod" v-for="produto in produtos">
    <img :src="produto.photoUrl" class="imgprod" />
    <div class="linha"></div>
    <p>{{ produto.name }}</p>
    <h3>R$ {{ produto.price }}</h3>
    <p>Preço médio</p>
    <button class="butloja">Ver na loja ></button>
  </div>
</template>
<style>
.divperfil {
  border-radius: 50%;
  height: 75px;
  width: 75px;
  display: inline-block;
  margin-left: 5%;
}
.imgperfil {
  border-radius: 322.5px;
}
.imgprod {
  border-radius: 27px 27px 0px 0px;
}
.butloja {
  color: blue;
}
.divprod {
  height: 300px;
  width: 200px;
  border: 1px solid black;
  border-radius: 30px;
  margin-left: 10%;

  margin-top: 30px;
  font-size: 15px;
  text-align: center;
  display: inline-block;
}
.linha {
  width: 100%;
  border: 1px solid #000;
}
</style>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "Perfil",
  data: () => {
    return {
      perfils: [
        {
          fotoUrl:
            "https://64.media.tumblr.com/722191e82b56be5c137a09b2b8d8fda1/ba9e8015a7fc00b1-7f/s1280x1920/bfd8761b73395b066da3e1d884385cb19ee6bc9d.jpg",
        },
        {
          fotoUrl:
            "https://pbs.twimg.com/media/FPRVP5pXIBkEtFu?format=jpg&name=small",
        },
        {
          fotoUrl: "https://cdn-icons-png.flaticon.com/512/1251/1251263.png",
        },
        {
          fotoUrl: "https://cdn-icons-png.flaticon.com/512/3135/3135768.png",
        },
        {
          fotoUrl: "https://pbs.twimg.com/media/EcGdw6wXYAUrPu4.jpg",
        },
        {
          fotoUrl:
            "https://guildfinder.com.br/editgfwp/wp-content/uploads/2021/06/perfilicon.jpeg",
        },

        {
          fotoUrl:
            "https://i.pinimg.com/474x/1e/5d/80/1e5d8021a1eaa0b05441b4ba96a46471.jpg",
        },
        {
          fotoUrl:
            "https://st3.depositphotos.com/1006318/18030/v/450/depositphotos_180303520-stock-illustration-arabic-man-profile-avatar-icon.jpg",
        },
        {
          fotoUrl:
            "https://i.pinimg.com/474x/b3/3c/f5/b33cf5488bac1c04f86df2304d141bba.jpg",
        },
        {
          fotoUrl: "https://pbs.twimg.com/media/FIw5YGEVgAEvViZ.jpg:large",
        },
      ],
      produtos: [
        {
          name: "a ética que o ivair não tem",
          photoUrl:
            "https://www.saocarloscursos.com.br/admin/arquivos/noticias/6/large/etica-profissional-2.jpg",
          price: 56.99,
        },
        {
          name: "Cola da prova do Ivair",
          photoUrl:
            "https://noticiasdemogi.com.br/wp-content/uploads/2019/04/gabarito.jpg",
          price: 0.0,
        },
        {
          name: "Recuperação do Ivair",
          photoUrl:
            "https://novosalunos.com.br/wp-content/uploads/2018/06/151374-nota-ruim-por-que-voce-deveria-se-importar-com-desempenho-academico-768x512.jpg",
          price: 99.9,
        },
        {
          name: "Peruca do Corredato",
          photoUrl:
            "https://ichef.bbci.co.uk/news/640/amz/worldservice/live/assets/images/2016/02/10/160210041136_thumbnail_calvicie_640x360_thinkstock.jpg",
          price: 499.9,
        },
        {
          name: "Recuperação do Ivair",
          photoUrl:
            "https://novosalunos.com.br/wp-content/uploads/2018/06/151374-nota-ruim-por-que-voce-deveria-se-importar-com-desempenho-academico-768x512.jpg",
          price: 99.9,
        },
        {
          name: "Peruca do Corredato",
          photoUrl:
            "https://ichef.bbci.co.uk/news/640/amz/worldservice/live/assets/images/2016/02/10/160210041136_thumbnail_calvicie_640x360_thinkstock.jpg",
          price: 499.9,
        },
      ],
    };
  },
});
</script>
