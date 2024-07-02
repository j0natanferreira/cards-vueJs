<template>
  <section>
    <CardsComponent
      v-for="user in users"
      :key="user.id"
      :avatar="user.avatar"
      :name="user.name"
      :description="user.description"
    />
  </section>
</template>

<script>
import CardsComponent from "./CardsComponent.vue";
export default {
  name: "SectionComponent",
  components: {
    CardsComponent,
  },
  data() {
    return {
      users: [
        {
          id: 1,
          avatar:
            "https://cajamar.sp.gov.br/noticias/wp-content/uploads/sites/2/2021/08/site-vacinacao-26-anos.png",
          name: "José Francisco",
          description:
            "Olá meu nome é José, sou uma pessoa seria e compromotido, vamos conversar mais.",
        },
        {
          id: 2,
          avatar: "https://tm.ibxk.com.br/2019/02/17/17124052466014.jpg",
          name: "João Silva",
          description:
            "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Molestias commodi eveniet.",
        },
        {
          id: 3,
          avatar:
            "https://i.pinimg.com/236x/4c/20/2b/4c202b6376037a5fc660a6c7b6e55661.jpg",
          name: "Maria de Souza",
          description:
            "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Molestias commodi eveniet.",
        },
      ],
    };
  },
};
</script>

<style scoped>
section {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
  overflow: auto;
}
</style>