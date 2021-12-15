<template>
  <div>
    <h1>Teste</h1>
    <h5>{{ nome }}</h5>
    <ul>
      <li v-for="prod in produtos" :key="prod.id">
        {{ prod.nome }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "ListagemPage",
  layout: "teste",
  data() {
    return {
      nome: "Eduardo Motton",
      produtos: [
        { id: 1, nome: "geladeira" },
        { id: 2, nome: "televisão" },
        { id: 3, nome: "cadeira" },
      ],
    };
  },
};
</script>
